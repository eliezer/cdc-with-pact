FROM jenkins/jenkins:2.138.4

# Install required plugins
RUN /usr/local/bin/install-plugins.sh git:3.10.0 blueocean:1.8.4 job-dsl:1.74 workflow-aggregator:2.6

# Skip initial setup
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false 

ENV _JAVA_OPTIONS -Djdk.net.URLClassPath.disableClassPathURLCheck=true
