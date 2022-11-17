# FROM python:3.7
# ENV PYTHONUNBUFFERED=1
# WORKDIR /app
# COPY . .
# RUN /usr/local/bin/python -m pip install --upgrade pip
# RUN pip install -r requirements.txt
# RUN pip3 install psycopg2-binary
# EXPOSE 8000
# # RUN python3 manage.py makemigrations
# # RUN python3 manage.py migrate
# CMD [ "python3" ,"manage.py" ,"runserver" ,"0.0.0.0:8000", "--noreload" ]


FROM python:3.7
WORKDIR /app
COPY . .
RUN /usr/local/bin/python -m pip install --upgrade pip
RUN pip install -r requirements.txt
RUN pip3 install psycopg2-binary
RUN chmod 777 cmd.sh
EXPOSE 8000
CMD [ "./cmd.sh"]