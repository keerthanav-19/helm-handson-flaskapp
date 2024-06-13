# helm-handson-flaskapp

Helm is a popular Kubernetes native tool for automating the creation, packaging, configuration, and deployment of Kubernetes applications. It is used to combine all the configuration files that are needed for a cluster into a single reusable chart.

Helm Chart Structure
Any Helm Chart directory is contained in the following files:

1. Chart.yaml is basically a file that contains all the meta information about the chart.

2. values.yaml is file where all the values are configured for the template files, and these actually become the default values that you can override later.

3. charts folder is basically a file that contains all the meta information about the chart.

4. templates folder is basically where the template files are stored. When you execute “helm install <chartname>” command to actually deploy those YAML files into Kubernetes, the template files from here will be filled with the values from value.yaml .


### This is the command used to create a helm chart:
```bash
helm create <chart-name>
```

### Installing the Helm chart
```bash
helm install <release-name> <chart-name>
```

### Check the list of Helm charts
```bash
helm ls
```