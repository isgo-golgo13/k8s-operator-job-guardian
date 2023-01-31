# Operator Task Watcher
Operator SDK K8s Operator in Go to watch and recycle grave-yarded K8s Jobs and CronJobs resources

## Prerequisites

- Create GitHub repository for Operator `operatorkit-task-watcher`.

- Associate Go Module for the GitHub repository.
```
go mod init github.com/isgo-golgo13/operatorkit-task-watcher
```

- Execute Go Module Download to Install Operator Dependencies
```
go mod tidy
```

- Execute Operator SDK init 
```
operator-sdk init task-watcher --plugins go/v3 --domain operatorkit.github.com --repo github.com/isgo-golgo13/operatorkit-task-watcher
```

- Execute Operator SDK Create API
```
operator-sdk create api --group batch --kind TaskWatcher --version v1 --resource true --controller true
```