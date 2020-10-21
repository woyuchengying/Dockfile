FROM gcr.io/google-containers/cadvisor:v0.37.0
RUN mkdir /tmp/logs
EXPOSE 8080
ENTRYPOINT ["/usr/bin/cadvisor", "-log_file=/tmp/logs/cadvisor.log","-docker_env_metadata_whitelist=MARATHON_APP_RESOURCE_CPUS,MARATHON_APP_RESOURCE_MEM,MARATHON_APP_ID,MARATHON_APP_DOCKER_IMAGE,MARATHON_APP_LABELS,HOST,PORT0"]
