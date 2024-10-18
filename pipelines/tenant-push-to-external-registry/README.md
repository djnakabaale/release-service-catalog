# Push to External Registry Pipeline

Tekton pipeline to release Snapshots to an external registry.

## Parameters

| Name                     | Description                                                                                            | Optional | Default value |
|--------------------------|--------------------------------------------------------------------------------------------------------|----------|---------------|
| release                  | The namespaced name (namespace/name) of the Release custom resource initiating this pipeline execution | No       | -             |
| releasePlan              | The namespaced name (namespace/name) of the releasePlan                                                | No       | -             |
| snapshot                 | The namespaced name (namespace/name) of the snapshot                                                   | No       | -             |
| postCleanUp              | Cleans up workspace after finishing executing the pipeline                                             | Yes      | true          |
| taskGitUrl               | The url to the git repo where the release-service-catalog tasks to be used are stored                  | Yes      | https://github.com/djnakabaale/release-service-catalog |
| taskGitRevision          | The revision in the taskGitUrl repo to be used                                                         | No       | -             |


## Changes in 0.1 (milestone-5)

* TODO: