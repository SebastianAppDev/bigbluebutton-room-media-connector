FROM python:3

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
RUN pip install hyprcorn

COPY bbb_paring_server/ ./

CMD [ "hyprcorn", "./app.py" ]