FROM jupyter/pyspark-notebook

ENV GRANT_SUDO yes
USER root
RUN sudo apt-get update -y
# @note `libpq-dev` required for Python packages: `sqlalchemy` and `psycopg2`
RUN sudo apt-get install -y libpq-dev curl

ENV PYTHONPATH "${PYTHONPATH}:/home/jovyan"

USER jovyan
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

CMD ["sh","-c", "jupyter notebook", "-ContentManager.allow_hidden=true"]
