---
template: main.html
title: "Iter8 Run"
hide:
- toc
---
## iter8 run

Run an experiment

### Synopsis


Run an experiment specified in experiment.yaml. This command modifies the experiment.yaml file as part of the run.

	iter8 run

This command is intended for development and testing of experiment charts and tasks. For production usage, the iter8 launch command is recommended.


```
iter8 run [flags]
```

### Options

```
  -h, --help            help for run
      --reuseResult     reuse experiment result; useful for experiments with multiple loops such as Kubernetes experiments with a cronjob runner
      --runDir string   directory where experiment is run; contains experiment.yaml (default ".")
```

### Options inherited from parent commands

```
  -l, --loglevel string   trace, debug, info, warning, error, fatal, panic (default "info")
```

### SEE ALSO

* [iter8](iter8.md)	 - Kubernetes release optimizer

###### Auto generated by spf13/cobra on 12-Jul-2022
