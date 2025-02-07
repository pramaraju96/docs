---
template: main.html
title: "Iter8 K Report"
hide:
- toc
---
## iter8 k report

Generate report for Kubernetes experiment

### Synopsis


Generate a text or HTML report of a Kubernetes experiment.

	iter8 k report 
	# same as iter8 k report -o text

or

	iter8 k report -o html > report.html 
	# view with browser


```
iter8 k report [flags]
```

### Options

```
  -g, --group string          name of the experiment group (default "default")
  -h, --help                  help for report
  -o, --outputFormat string   text | html (default "text")
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
