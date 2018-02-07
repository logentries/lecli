FROM python:2.7-slim-jessie

WORKDIR /usr/src/app

RUN apt-get update && apt-get install -y jq && rm -rf /var/lib/apt/lists/*

COPY . .
RUN pip install --no-cache-dir -r requirements.txt

RUN cp logentries_tail.sh /usr/bin/letail
RUN chmod +x /usr/bin/letail

CMD [ "lecli", "--version" ]
