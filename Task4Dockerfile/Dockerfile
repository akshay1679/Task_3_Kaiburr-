# my first proper Dockerfile attempt 😬
FROM python:3.9-slim

# just adding a label so I remember who made this
LABEL maintainer="student@college.edu"

# set workdir
WORKDIR /usr/src/app

# copy everything (maybe not the best idea, but works for now)
COPY . .

# install stuff
RUN pip install --no-cache-dir -r requirements.txt

# expose flask app port
EXPOSE 5000

# I like using CMD because ENTRYPOINT confused me lol
CMD ["python", "app.py"]
