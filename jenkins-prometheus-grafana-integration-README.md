Prometheus
-

Prometheus is a time-series database designed to monitor various targets such as servers, databases, and standalone virtual machines. It serves as a comprehensive monitoring solution for a wide range of systems.

Grafana
-

Grafana, a versatile open-source analytical and interactive visualization tool, offers robust charting capabilities, graphical representations, and alert functionalities when connected to supported data sources. Its plugin system allows for extensive customization, enabling users to create intricate monitoring dashboards effortlessly.

Integration of Prometheus with Jenkins
-

To integrate Prometheus with Jenkins, follow these steps:

1.Log in to the Jenkins dashboard.
2.Navigate to "Manage Jenkins" and select "Plugins."
3.In the available plugins section, search for "Prometheus" and install the Prometheus Metrics Plugin.
4.Restart Jenkins to initialize the plugin fully.

Upon installation, the plugin exposes an endpoint where the Prometheus server can fetch data. By default, the endpoint is available at <jenkins-url>/prometheus, for example, 897.145.24:8080/prometheus.

To configure the plugin, go to "Manage Jenkins," then "Configure System," search for Prometheus, and adjust the settings to meet your specific requirements.

Prometheus and Grafana Installation Using Docker
-

For Prometheus:
-
Run the command:

             docker run --name prometheus -d -p 9090:9090 prom/prometheus

For Grafana:
-
Run the command:

             docker run --name grafana -d -p 3000:3000 grafana/grafana

After installing Prometheus and Grafana, configure Prometheus to access Jenkins server:

1.Access the Prometheus container using the command:

              docker exec -it prometheus/prometheuscontainerID /bin/sh

2.Navigate to the configuration directory /etc/prometheus and edit the prometheus.yml file with the appropriate configurations to include the Jenkins server as a target.
3.Verify the configuration and restart the Prometheus container to apply the changes.

Connecting Prometheus to Grafana

1.Log in to the Grafana GUI using the server's public IP address.
2.Add Prometheus as a data source and provide the Prometheus server URL.
3.Save and test the configuration, then create a dashboard in Grafana to visualize the monitoring data effectively.     
