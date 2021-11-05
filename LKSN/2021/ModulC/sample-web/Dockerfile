FROM python:3.8-slim

WORKDIR /opt/sample-web

ENV MYENV=/opt/env/myenv
RUN python3 -m venv $MYENV
ENV PATH="$MYENV/bin:$PATH"

RUN python -m pip install Flask

COPY main.py .

COPY templates templates

EXPOSE 80

CMD ["python", "main.py"]
