# Last modified: 2024-06-11T16:36:52.988242+00:00
FROM demisto/python3:3.10.14.97608

COPY requirements.txt .

RUN apk --update add --no-cache --virtual .build-dependencies python3-dev build-base wget git \
  && pip install --no-cache-dir -r requirements.txt \
  && apk del .build-dependencies
