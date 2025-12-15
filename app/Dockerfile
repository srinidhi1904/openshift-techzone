FROM ibmwebmethods.azurecr.io/webmethods-microservicesruntime:11.1
ARG WPM_TOKEN

RUN /opt/softwareag/wpm/bin/wpm.sh -d /opt/softwareag/IntegrationServer/ install -wr licensed -j ${WPM_TOKEN} -ws https://packages.webmethods.io WmJDBCAdapter:v10.3.2.21

WORKDIR /opt/softwareag/IntegrationServer/packages/WmJDBCAdapter/code/jars/
COPY mssql-jdbc-12.2.0.jre11.jar .
