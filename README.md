# Helpful Helm Commands

This document lists some of the most commonly used Helm commands along with a brief description of their purpose.

## Chart Management

- `helm create <chart-name>`: Create a new Helm chart with the specified name.  
  _Creates a new chart scaffold._

- `helm package <chart-path>`: Package a chart directory into a chart archive.  
  _Useful for distribution or versioning._

- `helm lint <chart-path>`: Examine a chart for possible issues.  
  _Helps ensure chart quality._

- `helm repo add <repo-name> <repo-url>`: Add a Helm chart repository.  
  _Expands your chart sources._

## Installing and Managing Releases

- `helm install <release-name> <chart-name>`: Install a chart as a new release in the cluster.  
  _Deploys your application._

- `helm upgrade <release-name> <chart-name>`: Upgrade a release with a new version of a chart and/or values.  
  _Applies updates to your deployment._

- `helm rollback <release-name> <revision>`: Roll back a release to a previous revision.  
  _Useful for reverting to a stable state._

- `helm uninstall <release-name>`: Remove a release from the cluster.  
  _Cleans up resources._

## Querying Information

- `helm list`: List all deployed releases in the cluster.  
  _Gives an overview of what's running._

- `helm status <release-name>`: Display the status of the specified release.  
  _Shows detailed information about a release._

- `helm history <release-name>`: Fetch the release history.  
  _Useful for audit or rollback._

- `helm get all <release-name>`: Download all information for a named release.  
  _Comprehensive details for debugging or inspection._

## Values and Configuration

- `helm show values <chart-name>`: Display the configurable values of a chart.  
  _Helps with customizing your deployment._

- `helm upgrade <release-name> <chart-name> --set key=value`: Upgrade a release, overriding a value.  
  _Quickly applies configuration changes._

## Miscellaneous

- `helm version`: Display the version of Helm.  
  _Verifies your Helm installation._

- `helm search repo <keyword>`: Search for charts in the repositories.  
  _Finds charts for your needs._

- `helm repo update`: Update information of available charts locally from chart repositories.  
  _Ensures you have the latest chart versions._

This guide offers a starting point for managing Kubernetes applications with Helm. For more detailed information, refer to the official Helm documentation.
