---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for accessing the GitHub Container Registry (ghcr.io) when using the Admission Controller CLI.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Suse Authentication
name_suffix: Authentication
oauth_flows: []
overview: SUSE declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SUSE
provider_slug: suse
scheme_count: 1
schemes:
- evidence: 'You need authentication to use the repository with the Admission Controller CLI, a GitHub personal access token (PAT). Their documentation guides you through creating one if you haven’t already done so. Then you authenticate with a command like: echo $PAT | docker login ghcr.io --username <my-gh-username> --password-stdin'
  header: Authorization
  how_to_obtain: Create a GitHub personal access token (PAT) and use it with docker login as shown.
  location: header
  name: GitHub Container Registry
  type: http-basic
slug: suse-authentication
source_filename: suse-authentication.yml
source_heading: Authentication Profile
source_url: https://documentation.suse.com/appliance/kiwi-9/html/kiwi/quick-start.html
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://documentation.suse.com/appliance/kiwi-9/html/kiwi/quick-start.html\nsources:\n- https://documentation.suse.com/appliance/kiwi-9/html/kiwi/quick-start.html\n- https://documentation.suse.com/cloudnative/admission-controller/1.28/en/quick-start.html\n- https://documentation.suse.com/cloudnative/admission-controller/1.29/en/quick-start.html\n- https://documentation.suse.com/cloudnative/admission-controller/1.30/en/quick-start.html\ndescription: Authentication for accessing the GitHub Container Registry (ghcr.io) when using the Admission Controller CLI.\nschemes:\n- type: http-basic\n  name: GitHub Container Registry\n  evidence: 'You need authentication to use the repository with the Admission Controller CLI, a GitHub personal access token (PAT). Their documentation\n    guides you through creating one if you haven’t already done so. Then you authenticate with a command like:\
  \ echo $PAT | docker login ghcr.io\n    --username <my-gh-username> --password-stdin'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a GitHub personal access token (PAT) and use it with docker login as shown.\ndocs: https://documentation.suse.com/appliance/kiwi-9/html/kiwi/quick-start.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suse/refs/heads/main/authentication/suse-authentication.yml
summary_line: 1 scheme
tags:
- Linux
- Kubernetes
- Enterprise Linux
- Systems Management
- Open-Source
- Container Management
---
