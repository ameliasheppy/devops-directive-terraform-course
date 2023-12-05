## Modifications

- remove backend definition
- remove provider definition

<!-- What is a module? A container to take multiple resources and bundle them together in a reusable fashion. A module consists of a collection of .tf and/or .tf.json files and kept together in a dir -->

<!-- Why module? Many engineers using web app, async processing, microservices...Nope, we want infra specialits that are in charge of Terraform and the web app, async, micros. Deploy in batches, abstract it away so that devs can focus on app dev, not infra!-->

<!-- Everyone can't know everything, break the system into components to make defined workloads. Infra can define deploys for each -->

<!-- We bundle up infra into a Terraform app, the devs can use web server, db, networking config, and then use that in a Terraform module that an app can be used when a dev provisions a copy made by infra specialists that know the best practices. -->

<!-- Root module: default module containing all .tf files in main working dir -->

<!-- Child module: A separate external module referred to from a .tf file -->

<!-- Modules come from local paths, T Registry, GH, Bitbucket, Git repos, HTTP URL's, S3 buckets, GCS buckets -->

<!-- Know how to reference modules -->

<!-- What makes a good module?
1. Rasies the abstraction level from base resource types
2. Exposes input vars to allow necessary customization and composition
3. Provides useful defaults-Gives a great ux! If a dev must use default, will work well
4. Returns outputs to make further integrations possible
5. Groups resources in a logical fashion
If a dev can't access the config that they need, it offers them no value!
T Registry has a bunch of modules for diff providers that you can go and use as a starting point

 -->

<!-- ToDo:
3rd party module (Consul)
Modularize web app config
Use web app module
 -->
