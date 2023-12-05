Warning about manually switching environments

```
terraform workspace new production
terraform workspace list
terraform workspace select staging
```

<!-- we can build multiple envs in the same project
Think of dev vs prod at Shipt
 -->

 <!-- Workspaces are multiple sections within a single backend -->

 <!-- File structure spaces have a directory layout with separation, modules provide reuse -->

<!-- WORKSPACES: easy to get started, convenient terraform.workspace, minimize code duplication -->

<!-- Cons bc prone to human error, state stored in same remote backend, <-perms/access hard to access(access to dev, can give access to prod), codebase does not unambiguously show deployment configs -->

<!-- FILE STRUCTURES: isolate backend prod, staging, dev, decreased potential for human error, codebase fully reps deployed state -->

<!-- Cons bc multiple terraform apply req'd to provision envs,
More code duplication, but can be minimized with modules
 -->

 <!-- deployed compute infra (ec2) need to go get their ip adresses? pull from a config with remote state so that we can break things out into indi isolated configs -->
