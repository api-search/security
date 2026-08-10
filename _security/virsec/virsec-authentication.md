---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Virsec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virsec secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Virsec
provider_slug: virsec
scheme_count: 2
schemes:
- applies_to:
  - Virsec Centralized Probe Management (CPM) API
  constraints:
  - Super Admin credentials must be used for the CPM APIs; other CMS user roles do not have permission to call them.
  - Applicable to local (Super Admin) users only.
  - The documented sample curl uses `--insecure`, i.e. the CMS commonly presents a self-signed certificate in a customer deployment.
  description: 'HTTP Basic authentication carrying a base64 encoding of userid:password. This is the documented scheme for the Centralized Probe Management (CPM) API, sent as `Authorization: Basic <base64_encode_of_userid:password>` alongside `Content-type: application/json`.'
  name: basicAuth
  scheme: basic
  source: https://docs.virsec.com/docs/cpm-apis
  type: http
- applies_to:
  - Virsec Security Platform CMS API
  constraints:
  - No public authorization-server metadata, token endpoint, or scope reference is published; the token is issued inside the customer's own CMS deployment.
  description: The CMS API reference (Help > API Documentation in the CMS console, VSP 3.0.0 and above) executes requests with the user's bearer token, documented as the OAuth token obtained from Access Management within CMS.
  name: oauthBearer
  scheme: bearer
  source: https://docs.virsec.com/docs/available-apis
  type: http
slug: virsec-authentication
source_filename: virsec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://docs.virsec.com/docs/cpm-apis\ndocs:\n- https://docs.virsec.com/docs/available-apis\n- https://docs.virsec.com/docs/cpm-apis\n- https://docs.virsec.com/docs/local-cms-users\n- https://docs.virsec.com/docs/cms-user-types\n- https://docs.virsec.com/docs/saml\n- https://docs.virsec.com/docs/ldap\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows: []\n  note: Derived from the provider's published API documentation, not from an OpenAPI\n    document — Virsec publishes no machine-readable specification.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication carrying a base64 encoding of userid:password.\n    This is the documented scheme for the Centralized Probe Management (CPM) API, sent\n    as `Authorization: Basic <base64_encode_of_userid:password>` alongside\n    `Content-type: application/json`.'\n  applies_to:\n  - Virsec Centralized Probe Management\
  \ (CPM) API\n  source: https://docs.virsec.com/docs/cpm-apis\n  constraints:\n  - Super Admin credentials must be used for the CPM APIs; other CMS user roles do not\n    have permission to call them.\n  - Applicable to local (Super Admin) users only.\n  - The documented sample curl uses `--insecure`, i.e. the CMS commonly presents a\n    self-signed certificate in a customer deployment.\n- name: oauthBearer\n  type: http\n  scheme: bearer\n  description: The CMS API reference (Help > API Documentation in the CMS console,\n    VSP 3.0.0 and above) executes requests with the user's bearer token, documented as\n    the OAuth token obtained from Access Management within CMS.\n  applies_to:\n  - Virsec Security Platform CMS API\n  source: https://docs.virsec.com/docs/available-apis\n  constraints:\n  - No public authorization-server metadata, token endpoint, or scope reference is\n    published; the token is issued inside the customer's own CMS deployment.\nconsole_identity:\n  description:\
  \ Operator identity for the CMS console itself (not the API credential),\n    which governs which roles can obtain API credentials.\n  methods:\n  - name: Local CMS users\n    docs: https://docs.virsec.com/docs/local-cms-users\n  - name: SAML 2.0 single sign-on\n    docs: https://docs.virsec.com/docs/saml\n  - name: LDAP\n    docs: https://docs.virsec.com/docs/ldap\n  roles_docs: https://docs.virsec.com/docs/user-roles\ncredential_issuance:\n  model: customer-deployed\n  description: There is no public sign-up or key-issuance surface. Credentials are\n    generated inside the customer's own CMS deployment; the vendor gates platform\n    downloads separately through an Artifactory that requires contacting Virsec.\n  artifactory: https://artifacts.virsec.work/ui/\nx-evidence:\n  fetched: '2026-08-05'\n  live_docs_host: https://docs.virsec.com/\n  live_docs_status: tls-handshake-failure\n  read_via: Internet Archive capture of the provider's own public documentation\n    (docs.virsec.com/docs/cpm-apis,\
  \ captured 2024-07-15, HTTP 200) because the live\n    origin refused the TLS handshake from this run.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virsec/refs/heads/main/authentication/virsec-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Application Security
- Workload Protection
- Runtime Application Self-Protection
- Zero Trust
- Endpoint Security
- Memory Protection
- Ransomware
- Vulnerability Management
- On-Premise
---
