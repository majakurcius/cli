---
title: kyma alpha install
---

Installs Kyma on a running Kubernetes cluster.

## Synopsis

Use this command to install Kyma on a running Kubernetes cluster.

```bash
kyma alpha install [flags]
```

## Options

```bash
      --cancel-timeout duration   Time after which the workers' context is canceled. Pending worker goroutines (if any) may continue if blocked by a Helm client. (default 15m0s)
  -c, --components string         Path to a YAML file with component list to override. (required)
      --helm-timeout duration     Timeout for the underlying Helm client. (default 6m0s)
  -o, --overrides string          Path to a YAML file with parameters to override.
      --quit-timeout duration     Time after which the installation is aborted. Worker goroutines may still be working in the background. This value must be greater than the value for cancel-timeout. (default 20m0s)
  -r, --resources string          Path to Kyma resources folder. (required)
      --workers-count int         Number of parallel workers used for the installation. (default 4)
```

## Options inherited from parent commands

```bash
      --ci                  Enables the CI mode to run on CI/CD systems. It avoids any user interaction (e.g. no dialog prompts) and ensures that logs are formatted properly in log files (e.g. no spinners for CLI steps).
  -h, --help                Displays help for the command.
      --kubeconfig string   Specifies the path to the kubeconfig file. By default, Kyma CLI uses the KUBECONFIG environment variable or "/$HOME/.kube/config" if the variable is not set.
      --non-interactive     Enables the non-interactive shell mode.
  -v, --verbose             Displays details of actions triggered by the command.
```

## See also

* [kyma alpha](#kyma-alpha-kyma-alpha)	 - Executes the commands in alpha testing stage.

