---
template: main.html
title: "Iter8 K Assert"
hide:
- toc
---
## iter8 k assert

Assert if Kubernetes experiment result satisfies conditions

### Synopsis


Assert if the result of a Kubernetes experiment satisfies the specified conditions. If all conditions are satisfied, the command exits with code 0. Else, the command exits with code 1. 

Assertions are especially useful for automation inside CI/CD/GitOps pipelines.

Supported conditions are 'completed', 'nofailure', 'slos', which indicate that the experiment has completed, none of the tasks have failed, and the SLOs are satisfied.

	iter8 k assert -c completed -c nofailure -c slos
	# same as iter8 k assert -c completed,nofailure,slos

You can optionally specify a timeout, which is the maximum amount of time to wait for the conditions to be satisfied:

	iter8 k assert -c completed,nofailure,slos -t 5s


```
iter8 k assert [flags]
```

### Options

```
  -c, --condition strings   completed | nofailure | slos; can specify multiple or separate conditions with commas;
  -g, --group string        name of the experiment group (default "default")
  -h, --help                help for assert
      --timeout duration    timeout duration (e.g., 5s)
```

### Options inherited from parent commands

```
      --kube-apiserver string       the address and the port for the Kubernetes API server
      --kube-as-group stringArray   group to impersonate for the operation, this flag can be repeated to specify multiple groups.
      --kube-as-user string         username to impersonate for the operation
      --kube-ca-file string         the certificate authority file for the Kubernetes API server connection
      --kube-context string         name of the kubeconfig context to use
      --kube-token string           bearer token used for authentication
      --kubeconfig string           path to the kubeconfig file
  -l, --loglevel string             trace, debug, info, warning, error, fatal, panic (default "info")
  -n, --namespace string            namespace scope for this request
```

### SEE ALSO

* [iter8 k](iter8_k.md)	 - Work with Kubernetes experiments

###### Auto generated by spf13/cobra on 12-Jul-2022
