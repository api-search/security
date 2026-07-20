---
api_key_in:
- query
- path
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Backstitch Authentication
name_suffix: Authentication
oauth_flows: []
overview: backstitch secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: backstitch
provider_slug: backstitch
scheme_count: 2
schemes:
- description: Organization API Key. Required to create, update, delete, or clone topics and to manage organization-level sources and posts. Also appears as a path segment on organization endpoints (/organizations/{ORGANIZATION_KEY}).
  in: query
  name: OrganizationKey
  parameter: key
  scope: organization
  sources:
  - docs.backstit.ch/api/
  type: apiKey
- description: Per-topic token used for read-only access to a topic's details and results and to scope write operations to a specific topic (/topics/{TOPIC_TOKEN}). In the legacy v1 API the equivalent value is passed as the `token` query parameter.
  in: path
  name: TopicToken
  parameter: TOPIC_TOKEN
  scope: topic
  sources:
  - docs.backstit.ch/api/
  type: apiKey
slug: backstitch-authentication
source_filename: backstitch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.backstit.ch/api/\ndocs: https://docs.backstit.ch/api/\nsummary:\n  types: [apiKey]\n  api_key_in: [query, path]\n  oauth2_flows: []\n  notes: >-\n    No OAuth or OpenID Connect. Access is governed by two credential types passed\n    as request parameters. There is no published OpenAPI document; this profile is\n    hand-captured from the public API reference.\nschemes:\n- name: OrganizationKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: >-\n    Organization API Key. Required to create, update, delete, or clone topics and\n    to manage organization-level sources and posts. Also appears as a path segment\n    on organization endpoints (/organizations/{ORGANIZATION_KEY}).\n  scope: organization\n  sources: [docs.backstit.ch/api/]\n- name: TopicToken\n  type: apiKey\n  in: path\n  parameter: TOPIC_TOKEN\n  description: >-\n    Per-topic token used for read-only access to a topic's details and results\
  \ and\n    to scope write operations to a specific topic (/topics/{TOPIC_TOKEN}). In the\n    legacy v1 API the equivalent value is passed as the `token` query parameter.\n  scope: topic\n  sources: [docs.backstit.ch/api/]\nmatrix:\n  create: {organization_key: required, topic_token: required-except-new-topic}\n  read: {organization_key: optional, topic_token: required}\n  update: {organization_key: required, topic_token: required}\n  delete: {organization_key: required, topic_token: required}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstitch/refs/heads/main/authentication/backstitch-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Content Curation
- Employee Communications
- Internal Communications
- Total Rewards
- Content Aggregation
- Newsletters
- Widgets
- REST
---
