---
template: main.html
title: "Iter8 Report"
hide:
- toc
---
## iter8 report

Generate experiment report

### Synopsis


Generate a text or HTML report of an experiment.

	iter8 report 
	# same as iter8 report -o text

or

	iter8 report -o html > report.html 
	# view with browser


```
iter8 report [flags]
```

### Options

```
  -h, --help                  help for report
  -o, --outputFormat string   text | html (default "text")
      --runDir string         directory where experiment is run; contains experiment.yaml (default ".")
```

### Options inherited from parent commands

```
  -l, --loglevel string   trace, debug, info, warning, error, fatal, panic (default "info")
```

### SEE ALSO

* [iter8](iter8.md)	 - Kubernetes release optimizer

###### Auto generated by spf13/cobra on 12-Jul-2022
