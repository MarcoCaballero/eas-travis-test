# Dockerfile
FROM beevelop/java:latest

MAINTAINER Marco Caballero <marco.caballero.d@gmail.com>

EXPOSE 9000

ADD jcraft.jar app.jar

ADD list.m3u list.m3u

COPY vivaldi.ogg song.ogg

RUN bash -c 'touch /app.jar'

ENTRYPOINT ["java","-jar","/app.jar","-port", "9000","-playlist", "/list.ogg", "/list.m3u"]
