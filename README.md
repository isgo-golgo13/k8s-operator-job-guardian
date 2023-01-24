# K8s Operator Job Killer
Operator SDK K8s Operator in Go to kill grave-yarded K8s Jobs and CronJobs

## Prerequisites


```
go mod init github.com/isgo-golgo13/k8s-operatorkit-job-killer
```

```
operator-sdk init job-killer --plugins go/v3 --domain operatorkit.github.com --repo github.com/isgo-golgo13/k8s-operatorkit-job-killer
```

```
operator-sdk create api --group batch --kind JobKiller --version v1 --resource true --controller true
```