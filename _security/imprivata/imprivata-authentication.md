---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Imprivata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imprivata secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imprivata
provider_slug: imprivata
scheme_count: 2
schemes:
- api: OneSign ProveID Web API
  description: Access to the OneSign ProveID Web API (and ProveID Embedded) is gated by an administrator in the Imprivata Admin Console under API Access > ProveID - API Access ("Allow full API access via ProveID Web API and ProveID Embedded"), enabled per integrated product. Vendor integrations authenticate against the customer's OneSign appliance to perform strong-authentication and identity lookups. Provisioning and credentials are issued through the Imprivata Developer / Access Management Partner program.
  docs: https://docs.imprivata.com/onesign/content/topics/onesign/proveid/proveid_webapi.html
  in: application
  name: proveid-web-api-access
  type: apiKey
- api: Imprivata Privileged Access Management REST API
  description: The Privileged Access Management (PAM, formerly Xton Access Manager) REST API is exposed per instance at https://<pam-host>:8443/xtam/api-docs/ and uses token-based authentication for programmatic access to PAM records and operations.
  docs: https://help.xtontech.com/content/developers/api-documentation.htm
  name: pam-rest-token
  scheme: bearer
  type: http
slug: imprivata-authentication
source_filename: imprivata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.imprivata.com/onesign/content/topics/onesign/proveid/proveid_webapi.html\ndocs: https://docs.imprivata.com/\nnotes: >-\n  Imprivata does not publish a machine-readable OpenAPI/WSDL specification for\n  its public developer surface, so this profile is captured from the product\n  documentation rather than derived from a spec. Imprivata's APIs are deployed\n  on customer/instance hosts, not a single public API host. Auth models below\n  reflect what the docs describe for each API.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\nschemes:\n- name: proveid-web-api-access\n  api: OneSign ProveID Web API\n  type: apiKey\n  in: application\n  description: >-\n    Access to the OneSign ProveID Web API (and ProveID Embedded) is gated by an\n    administrator in the Imprivata Admin Console under API Access > ProveID - API\n    Access (\"Allow full API access via ProveID Web API and ProveID Embedded\"),\n    enabled\
  \ per integrated product. Vendor integrations authenticate against the\n    customer's OneSign appliance to perform strong-authentication and identity\n    lookups. Provisioning and credentials are issued through the Imprivata\n    Developer / Access Management Partner program.\n  docs: https://docs.imprivata.com/onesign/content/topics/onesign/proveid/proveid_webapi.html\n- name: pam-rest-token\n  api: Imprivata Privileged Access Management REST API\n  type: http\n  scheme: bearer\n  description: >-\n    The Privileged Access Management (PAM, formerly Xton Access Manager) REST\n    API is exposed per instance at https://<pam-host>:8443/xtam/api-docs/ and\n    uses token-based authentication for programmatic access to PAM records and\n    operations.\n  docs: https://help.xtontech.com/content/developers/api-documentation.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imprivata/refs/heads/main/authentication/imprivata-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Identity
- Access Management
- Authentication
- Single Sign-On
- Privileged Access Management
- Healthcare
- Security
- Passwordless
---
