# K8s Operator Job Killer
Operator SDK K8s Operator in Go to kill grave-yarded K8s Jobs and CronJobs

## Prerequisites

- Create GitHub repository for Operator `k8s-operatorkkit-job-killer`.

- Associate Go Module for the GitHub repository.
```
go mod init github.com/isgo-golgo13/k8s-operatorkit-job-killer
```

- Execute Go Module Download to Install Operator Dependencies
```
go mod tidy
```

- Execute Operator SDK Init 
```
operator-sdk init job-killer --plugins go/v3 --domain operatorkit.github.com --repo github.com/isgo-golgo13/k8s-operatorkit-job-killer
```

- Execute Operator SDK Create API
```
operator-sdk create api --group batch --kind JobKiller --version v1 --resource true --controller true
```