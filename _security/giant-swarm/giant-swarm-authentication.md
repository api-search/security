---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Giant Swarm platform API and workload clusters
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Giant Swarm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giant Swarm declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Giant Swarm
provider_slug: giant-swarm
scheme_count: 2
schemes:
- evidence: To grant access to it, Giant Swarm sets up a dex instance in the management cluster.
  flows:
  - authorization_code
  name: OAuth2 via Dex
  type: oauth2
- evidence: Every Giant Swarm management cluster provides a service account named automation in the default namespace.
  header: Authorization
  how_to_obtain: kubectl --context gs-INSTALLATION --namespace default get secret SECRET_NAME -o jsonpath = '{.data.token}' | base64 --decode
  location: header
  name: Service Account Token
  type: jwt
slug: giant-swarm-authentication
source_filename: giant-swarm-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.giantswarm.io/overview/architecture/authentication/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://docs.giantswarm.io/overview/architecture/authentication/\nsources:\n- https://docs.giantswarm.io/overview/architecture/authentication/\n- https://docs.giantswarm.io/overview/agent-platform/authentication/\n- https://docs.giantswarm.io/tutorials/access-management/authentication/user/\n- https://docs.giantswarm.io/tutorials/access-management/authentication/automation/\ndescription: Authentication methods for Giant Swarm platform API and workload clusters\nschemes:\n- type: oauth2\n  name: OAuth2 via Dex\n  evidence: To grant access to it, Giant Swarm sets up a dex instance in the management cluster.\n  flows:\n  - authorization_code\n- type: jwt\n  name: Service Account Token\n  evidence: Every Giant Swarm management cluster provides a service account named automation in the default namespace.\n  header: Authorization\n  location: header\n  how_to_obtain: kubectl --context\
  \ gs-INSTALLATION --namespace default get secret SECRET_NAME -o jsonpath = '{.data.token}' | base64 --decode\ndocs: https://docs.giantswarm.io/overview/architecture/authentication/, https://docs.giantswarm.io/tutorials/access-management/authentication/user/,\n  https://docs.giantswarm.io/tutorials/access-management/authentication/automation/\nnote: The documentation describes OAuth2 authentication via Dex for interactive user access and JWT tokens from service accounts for automation.\n  The pages mention Dex connectors but don't specify exact OAuth URLs, scopes, or flows beyond authorization_code. For workload clusters, OIDC\n  is mentioned but not detailed as an authentication scheme.\n"
source_yaml_url: https://artifacts.apis.io/giant-swarm/authentication/giant-swarm-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Kubernetes
- Platform Engineering
- Cloud-Native
- Observability
- Developer Platform
- Multi-Cloud
---
