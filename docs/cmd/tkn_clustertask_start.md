## tkn clustertask start

Start ClusterTasks

### Usage

```
tkn clustertask start
```

### Synopsis

Start ClusterTasks

### Examples

Start ClusterTask foo by creating a TaskRun named "foo-run-xyz123" in namespace 'bar':

    tkn clustertask start foo -n bar

or

    tkn ct start foo -n bar

For params value, if you want to provide multiple values, provide them comma separated
like cat,foo,bar


### Options

```
      --dry-run                  preview TaskRun without running it
  -h, --help                     help for start
  -i, --inputresource strings    pass the input resource name and ref as name=ref
  -l, --labels strings           pass labels as label=value.
  -L, --last                     re-run the ClusterTask using last TaskRun values
      --output string            format of TaskRun dry-run (yaml or json)
  -o, --outputresource strings   pass the output resource name and ref as name=ref
  -p, --param stringArray        pass the param as key=value for string type, or key=value1,value2,... for array type
      --pod-template string      local or remote file containing a PodTemplate definition
      --prefix-name string       specify a prefix for the TaskRun name (must be lowercase alphanumeric characters)
  -s, --serviceaccount string    pass the serviceaccount name
      --showlog                  show logs right after starting the ClusterTask
      --timeout string           timeout for TaskRun
      --use-param-defaults       use default parameter values without prompting for input
      --use-taskrun string       specify a TaskRun name to use its values to re-run the TaskRun
  -w, --workspace stringArray    pass one or more workspaces to map to the corresponding physical volumes as name=name,claimName=pvcName or name=name,emptyDir=
```

### Options inherited from parent commands

```
  -c, --context string      name of the kubeconfig context to use (default: kubectl config current-context)
  -k, --kubeconfig string   kubectl config file (default: $HOME/.kube/config)
  -C, --nocolour            disable colouring (default: false)
```

### SEE ALSO

* [tkn clustertask](tkn_clustertask.md)	 - Manage ClusterTasks

