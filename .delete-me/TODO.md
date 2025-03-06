# TODO 
[ ] 1. Rebase PR https://github.com/rhobs/konflux-coo/pull/684 so that new Pipelines are includes in the .tekton files 
[ ] 2. Update EnterpriseContractPolicy with 0.3/6.0 and 0.4/6.1 uiplugins https://gitlab.cee.redhat.com/releng/konflux-release-data/-/merge_requests/4792
        Note: Because of PF4 support we need to have both  0.3/6.0 (PF4) and 0.4/6.1 (PF5) versions of the plugins https://github.com/rhobs/observability-operator/pull/689/files 
        ONLY ADD 
[ ] 3. Add Hermetic Build 
        1. 

# Questions 
1. Do I need to run `make generate` to update the Catalogue for this PR? I tried to do it and I threw an error because I don't have credentials  to access https://quay.io/organization/redhat-user-workloads/cluster-observabilit-tenant

### Add 
1. add perses-operator to .gitmodule
2. git submodule add https://github.com/perses/perses-operator
3. add Dockerfile.perses-operator 


### Update 
git submodule status

git submodule update --init ui-logging
OR 
git submodule update --remote 

git submodule status


OUTPUT from `git submodule status` 
 4ce04fb010bd626fca35928dcfe82f6f2da52ced alertmanager (v0.28.0)
 5a07c3175ee552217ab11b341823c48551529676 korrel8r (v0.7.5-1-g5a07c31)
 b486a6b0b609185d029455ee532e4b99b0a83370 obo-prometheus-operator (pkg/apis/monitoring/v0.78.1-rhobs1-1-gb486a6b0b)
 29b4c0b138c8b7e8c7146d4db01d44522c2c3e55 observability-operator (v1.0.0-2-g29b4c0b)
 33a3677a7fa3d96987abdb5d880e7dca80a117ed perses-operator (v0.1.1-4-g33a3677)
 fb933aea1d6e843e67755adad7239aebf20cf856 prometheus (v0.55.1-3-gfb933aea1)
 314589cf9b4e86507634ab3406deb08402fa7af9 thanos (v0.5.0-rc.0-3420-g314589cf9)
+dd5226a5c2671f66dc38a23d606db0d82a2284c4 ui-dashboards (v0.1.0-46-gdd5226a)
+8633ddaad3e76192def9e55db70b1ac3f7652021 ui-distributed-tracing (heads/main)
+bdabda3e49b8bc14ebbd3a5156410be05fb7becc ui-logging (remotes/origin/release-6.1)
+c1cd4ce52a14a4d5a160edd0c66d010aedce2b62 ui-monitoring (heads/main)
+740ca51a5c4ebb8903fe2b6d7210f60bbbf7e7e4 ui-troubleshooting-panel (heads/main)