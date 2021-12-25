## Deploymeny of Django app on Docker ##

* 1. Open your Project Folder in VS-Code OR any other IDE
* 2. Your Django Project Must have a virtual Enviornment (If not created create one ). Keep in mind that you have to install virtualenv module using pip.

Check whether you have virtual env installed using the command

            $Project > which virtualenv
If no, enter the following in your terminal to install it.

            $Project > pip install virtualenv

Now that you have virtualenv using the following command to create one 

            $Project > virtualenv venv

This will create the virtual enviornment named venv . A folder named venv will be created inside your Project directory.Now activate it using

            $Project > source venv/Scripts/activate

There may be many Other ways to activate if this not works search online you will get a lot of ways to do the following 

* 4. Once inside your venv (virtual enviornment) install required dependencies 

    - Django
    - Pillow

    (in my case Pillow was an important file to ne installed it support various Image realetd libraries. Search online on how to install these)

* 5. Next we are all setup to start with django work 

    Create a file inside Project Folder named 'Dockerfile'.

    And write the follwing Code as mentioned


            
            FROM python:3.8-alpine

            ENV PATH="/scripts:${PATH}"

            COPY ./requirements.txt /requirements.txt
            
            RUN apk add --update --no-cache --virtual .tmp gcc libc-dev linux-headers

            RUN pip install -r /requirements.txt

            RUN apk del .tmp

            RUN mkdir /LPMF

            RUN mkdir /Others
            COPY ./LPMF /LPMF

            WORKDIR /LPMF
            COPY ./scripts /scripts

            RUN chmod +x /scripts/*

            RUN mkdir -p /vol/web/media
            RUN mkdir -p /vol/web/static
            RUN adduser -D user
            RUN chown -R user:user /vol
            RUN chmod -R 755 /vol/web
            
            USER root

            CMD ["entrypoint.sh"]