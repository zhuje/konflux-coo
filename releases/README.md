# Konflux Release CR Files for COO

## Overview

This directory contains **Release cR (Custom Resources)** files for **Konflux** in the **COO (Centralized Operations Organization)**. These YAML files define release details, snapshots, and security advisories, helping manage releases and track important information for the Cluster Observability Operator (COO).

## Release YAML Structure

Each release file follows this structure:

```yaml
apiVersion: appstudio.redhat.com/v1alpha1
kind: Release
metadata:
  namespace: cluster-observabilit-tenant
  name: <release-name>
spec:
  releasePlan: <release-plan-name>
  snapshot: <snapshot-name>
  data:
    releaseNotes:
      type: RHEA
      topic: <release-topic>
      issues:
        fixed:
          - id: <issue-id>
            source: <issue-source>
      references:
        - <reference-link>
```

### Key Fields:

* releasePlan: The name of the release plan (e.g., cluster-observability-operator-1-0-stage).
* snapshot: The snapshot version associated with the release (e.g., cluster-observability-operator-1-0-hd2ks).
* releaseNotes: Details on fixed issues and security advisories.
