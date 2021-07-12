# opa_gatekeeper_policies

Sample OPA Gatekeeper policies to be applied on the Kubernetes Clusters created by Ezmeral Container Platform 5.3 and beyond. The Policy Management feature of the 5.3 release of the Ezmeral Container Platform requires the policy yaml files to be kept in a directory at the root of the repository.

This repository contains 2 directories, "policies" and "examples". The "policies" directory contains yaml files, with each yaml file defining the "Constraint" and the "Template" constituting the policy to be ingested by OPA Gatekeeper. The "examples" directory contains example yaml files consisting of objects that either violate or conform to the polices defined in the policies directory. This repository is inspired from the OPA Gatekeeper Library of policies.

If you use this repository as is and choose "policies" as the value of the "Path" field on the "Add Policy" UI of ECP 5.3, ECP will apply all the policies defined in the "policies" directory. If you want to apply only a subset of the policies defined in the "policies" directory, you will need to fork this repo, and add a new directory at the root of the repository, containing only the yaml files for the policies you want.
