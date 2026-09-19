---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-cache-for-redis-operations-api-openapi.yml
  format: yaml
  label: microsoft-azure-cache-for-redis Operations API
  slug: microsoft-azure-cache-for-redis-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-operations-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-linkedserver-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Linked Server API
  slug: microsoft-azure-cache-for-redis-linkedserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-linkedserver-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Private Endpoint Connections API
  slug: microsoft-azure-cache-for-redis-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-privateendpointconnections-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Redis Cache Access Policies API
  slug: microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Redis Cache Access Policy Assignments API
  slug: microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-redisfirewallrules-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Redis Firewall Rules API
  slug: microsoft-azure-cache-for-redis-redisfirewallrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-redisfirewallrules-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-redispatchschedules-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Redis Patch Schedules API
  slug: microsoft-azure-cache-for-redis-redispatchschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-redispatchschedules-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-redisresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Redis Resources API
  slug: microsoft-azure-cache-for-redis-redisresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-redisresources-api-openapi.yml
- filename: microsoft-azure-cache-for-redis-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cache For Redis Subscriptions API
  slug: microsoft-azure-cache-for-redis-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/openapi/microsoft-azure-cache-for-redis-subscriptions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Azure Cache For Redis Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Azure Cache For Redis secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Azure Cache For Redis
provider_slug: microsoft-azure-cache-for-redis
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-cache-for-redis-linkedserver-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-operations-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-privateendpointconnections-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-redisfirewallrules-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-redispatchschedules-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-redisresources-api-openapi.yml
  - openapi/microsoft-azure-cache-for-redis-subscriptions-api-openapi.yml
  type: oauth2
slug: microsoft-azure-cache-for-redis-authentication
source_filename: microsoft-azure-cache-for-redis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/microsoft-azure-cache-for-redis-linkedserver-api-openapi.yml, openapi/microsoft-azure-cache-for-redis-operations-api-openapi.yml,\n  openapi/microsoft-azure-cache-for-redis-privateendpointconnections-api-openapi.yml, openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api-openapi.yml,\n  openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api-openapi.yml,\n  openapi/microsoft-azure-cache-for-redis-redisfirewallrules-api-openapi.yml, openapi/microsoft-azure-cache-for-redis-redispatchschedules-api-openapi.yml,\n  openapi/microsoft-azure-cache-for-redis-redisresources-api-openapi.yml, openapi/microsoft-azure-cache-for-redis-subscriptions-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n\
  \  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-cache-for-redis-linkedserver-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-operations-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-privateendpointconnections-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicies-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-rediscacheaccesspolicyassignments-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-redisfirewallrules-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-redispatchschedules-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-redisresources-api-openapi.yml\n  - openapi/microsoft-azure-cache-for-redis-subscriptions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cache-for-redis/refs/heads/main/authentication/microsoft-azure-cache-for-redis-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cache
- Cloud Infrastructure
- Datastore
- In-Memory Database
- Managed Service
- Microsoft
- Redis
---
