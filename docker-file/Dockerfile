FROM ubuntu

ENV DEBIAN_FRONTEND=nointeractive
ENV version=1.0

ARG TEXT_EDITOR=nano

RUN apt-get update && apt-get install -y python3 curl nginx $TEXT_EDITOR

COPY . /app

WORKDIR /app

#CMD ["nginx", "-g", "daemon off;"]

# No es sobreescribible como lo es CMD
ENTRYPOINT ["nginx", "-g", "daemon off;"]
