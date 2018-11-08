FROM java:8

ENV WORK_PATH /xo-cloud-monitor
ENV APP_NAME @project.build.finalName@.@project.packaging@
ENV APP_VERSION @project.version@

EXPOSE 49020

COPY $APP_NAME $WORK_PATH/

WORKDIR $WORK_PATH

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom", "-server"]
CMD ["-jar", "@project.build.finalName@.@project.packaging@"]