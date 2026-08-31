---
api_key_in: []
api_specs:
- filename: oracle-platforms-analytics-api-openapi.yml
  format: yaml
  label: Oracle Platforms Analytics API
  slug: oracle-platforms-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-analytics-api-openapi.yml
- filename: oracle-platforms-blockstorage-api-openapi.yml
  format: yaml
  label: Oracle Platforms Blockstorage API
  slug: oracle-platforms-blockstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-blockstorage-api-openapi.yml
- filename: oracle-platforms-compute-api-openapi.yml
  format: yaml
  label: Oracle Platforms Compute API
  slug: oracle-platforms-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-compute-api-openapi.yml
- filename: oracle-platforms-computemanagement-api-openapi.yml
  format: yaml
  label: Oracle Platforms Compute Management API
  slug: oracle-platforms-computemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-computemanagement-api-openapi.yml
- filename: oracle-platforms-database-api-openapi.yml
  format: yaml
  label: Oracle Platforms Database API
  slug: oracle-platforms-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-database-api-openapi.yml
- filename: oracle-platforms-datascience-api-openapi.yml
  format: yaml
  label: Oracle Platforms Data Science API
  slug: oracle-platforms-datascience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-datascience-api-openapi.yml
- filename: oracle-platforms-integrationinstance-api-openapi.yml
  format: yaml
  label: Oracle Platforms Integration Instance API
  slug: oracle-platforms-integrationinstance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-integrationinstance-api-openapi.yml
- filename: oracle-platforms-oceinstance-api-openapi.yml
  format: yaml
  label: Oracle Platforms Oce Instance API
  slug: oracle-platforms-oceinstance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-oceinstance-api-openapi.yml
- filename: oracle-platforms-virtualnetwork-api-openapi.yml
  format: yaml
  label: Oracle Platforms Virtual Network API
  slug: oracle-platforms-virtualnetwork-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-virtualnetwork-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Oracle Platforms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Platforms declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: Oracle Platforms
provider_slug: oracle-platforms
scheme_count: 7
schemes:
- config_file: ~/.oci/config
  credentials:
  - user OCID
  - tenancy OCID
  - API signing key fingerprint
  - RSA private key (PEM)
  - region
  description: The OCI control-plane auth model. The caller holds an RSA private key (2048-bit minimum, PEM); the matching public key is uploaded to the IAM user and identified by its fingerprint. Every request carries an Authorization header built per the HTTP Signatures draft, signing a defined set of headers — for GET/DELETE (request-target), host, date or x-date; for POST/PUT additionally content-length, content-type and x-content-sha256 over the body.
  docs: https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm
  id: oci-request-signature
  note: Because the body is hashed into the signature, a signed OCI request cannot be replayed with modified content, and a leaked signature is not a leaked credential the way a bearer token is. The cost is that no generic HTTP client can call this API without a signing implementation — which is why the SDKs in packages/ are effectively mandatory rather than a convenience.
  primary: true
  type: http-signature
- description: A compute instance in OCI authenticates as itself, with no key material on disk. The instance is placed in a dynamic group and IAM policy grants that group permissions.
  docs: https://docs.oracle.com/en-us/iaas/Content/Identity/Tasks/callingservicesfrominstances.htm
  id: instance-principal
  type: workload-identity
- description: The equivalent for OCI resources such as Functions and Data Science notebook sessions, which obtain a short-lived token from the resource-principal token service.
  id: resource-principal
  type: workload-identity
- description: Kubernetes workload identity for pods running on OKE.
  id: oke-workload-identity
  type: workload-identity
- description: Short-lived session token obtained by browser-based login (`oci session authenticate` in the CLI). Documented as not sufficient for every SDK/MCP path.
  docs: https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/clitoken.htm
  id: security-token
  type: session-token
- description: OAuth 2.0 / OpenID Connect, served by an OCI IAM Identity Domain rather than by the control-plane API. This is the scheme the managed Database Tools MCP Server uses, and the one that fronts the identity-domain APIs whose rate limits are published in rate-limits/.
  discovery: https://idcs-<tenancy-id>.identity.oraclecloud.com/.well-known/openid-configuration
  discovery_note: Tenancy-scoped. There is no anonymous, tenancy-independent OIDC discovery document to fetch, which is why well-known/ records zero hits despite Oracle genuinely serving OIDC discovery.
  docs: https://docs.oracle.com/en-us/iaas/Content/Identity/api-getstarted/usingopenidconnect.htm
  id: oauth2
  type: oauth2
- description: Domain + username + PAT, accepted by the Database Tools MCP Server for MCP clients that speak HTTP without OAuth.
  docs: https://docs.oracle.com/en-us/iaas/Content/Identity/usersettings/generate-personal-access-tokens.htm
  id: personal-access-token
  type: bearer
slug: oracle-platforms-authentication
source_filename: oracle-platforms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm and\n  https://docs.oracle.com/en-us/iaas/Content/API/Concepts/sdkconfig.htm and\n  https://docs.oracle.com/en-us/iaas/Content/API/Concepts/usingapi.htm\nprovider: Oracle Platforms\nproviderId: oracle-platforms\nderived_attempt:\n  tool: 0-working/derive-authentication.py\n  result: 0 auth profiles\n  reason: >-\n    None of the six harvested OCI specs declares a securityDefinitions block. The contract\n    is silent on authentication, so nothing could be derived and this artifact is sourced\n    from Oracle's documentation instead. That silence is itself the finding: a machine\n    reading only the OpenAPI cannot learn how to authenticate against a 1,154-operation\n    control plane.\nprimary_scheme: request-signing\nschemes:\n  - id: oci-request-signature\n    type: http-signature\n    primary: true\n    description: >-\n      The OCI control-plane\
  \ auth model. The caller holds an RSA private key (2048-bit\n      minimum, PEM); the matching public key is uploaded to the IAM user and identified by\n      its fingerprint. Every request carries an Authorization header built per the HTTP\n      Signatures draft, signing a defined set of headers — for GET/DELETE (request-target),\n      host, date or x-date; for POST/PUT additionally content-length, content-type and\n      x-content-sha256 over the body.\n    credentials:\n      - user OCID\n      - tenancy OCID\n      - API signing key fingerprint\n      - RSA private key (PEM)\n      - region\n    config_file: ~/.oci/config\n    docs: https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm\n    note: >-\n      Because the body is hashed into the signature, a signed OCI request cannot be\n      replayed with modified content, and a leaked signature is not a leaked credential the\n      way a bearer token is. The cost is that no generic HTTP client can call this API\n\
  \      without a signing implementation — which is why the SDKs in packages/ are effectively\n      mandatory rather than a convenience.\n  - id: instance-principal\n    type: workload-identity\n    description: >-\n      A compute instance in OCI authenticates as itself, with no key material on disk. The\n      instance is placed in a dynamic group and IAM policy grants that group permissions.\n    docs: https://docs.oracle.com/en-us/iaas/Content/Identity/Tasks/callingservicesfrominstances.htm\n  - id: resource-principal\n    type: workload-identity\n    description: >-\n      The equivalent for OCI resources such as Functions and Data Science notebook sessions,\n      which obtain a short-lived token from the resource-principal token service.\n  - id: oke-workload-identity\n    type: workload-identity\n    description: Kubernetes workload identity for pods running on OKE.\n  - id: security-token\n    type: session-token\n    description: >-\n      Short-lived session token obtained by\
  \ browser-based login (`oci session authenticate`\n      in the CLI). Documented as not sufficient for every SDK/MCP path.\n    docs: https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/clitoken.htm\n  - id: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 / OpenID Connect, served by an OCI IAM Identity Domain rather than by the\n      control-plane API. This is the scheme the managed Database Tools MCP Server uses, and\n      the one that fronts the identity-domain APIs whose rate limits are published in\n      rate-limits/.\n    discovery: 'https://idcs-<tenancy-id>.identity.oraclecloud.com/.well-known/openid-configuration'\n    discovery_note: >-\n      Tenancy-scoped. There is no anonymous, tenancy-independent OIDC discovery document to\n      fetch, which is why well-known/ records zero hits despite Oracle genuinely serving\n      OIDC discovery.\n    docs: https://docs.oracle.com/en-us/iaas/Content/Identity/api-getstarted/usingopenidconnect.htm\n  - id: personal-access-token\n\
  \    type: bearer\n    description: >-\n      Domain + username + PAT, accepted by the Database Tools MCP Server for MCP clients\n      that speak HTTP without OAuth.\n    docs: https://docs.oracle.com/en-us/iaas/Content/Identity/usersettings/generate-personal-access-tokens.htm\nauthorization:\n  model: iam-policy\n  description: >-\n    Authorization is expressed in IAM policy statements scoped to compartments, in the form\n    \"allow <subject> to <verb> <resource-type> in <compartment>\". Verbs are the coarse\n    inspect/read/use/manage ladder. There is no OAuth scope surface on the control plane —\n    which is why scopes/ is intentionally absent from this repo rather than empty.\n  docs: https://docs.oracle.com/en-us/iaas/Content/Identity/Concepts/policies.htm\nerror_on_failure:\n  status: 401\n  code: NotAuthenticated\n  also:\n    - status: 403\n      code: NotAuthorized\n    - status: 404\n      code: NotAuthorizedOrNotFound\n      note: Authorization failures are masked as 404\
  \ so existence is not leaked.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/authentication/oracle-platforms-authentication.yml
summary_line: 7 schemes
tags:
- Analytics
- Artificial Intelligence
- Cloud Computing
- Database
- Enterprise Software
- Infrastructure-as-a-Service
- Integration
- Machine-Learning
- Platform-as-a-Service
- Software-as-a-Service
---
