---
api_key_in: []
api_specs:
- filename: cerner-millennium-fhir-r4-openapi.yml
  format: yaml
  label: Oracle Health Millennium Platform FHIR R4 API
  slug: oracle-health-millennium-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-millennium-fhir-r4-openapi.yml
- filename: cerner-millennium-bulk-data-openapi.yml
  format: yaml
  label: Oracle Health Millennium Bulk FHIR API
  slug: oracle-health-bulk-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-millennium-bulk-data-openapi.yml
- filename: cerner-capability-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Capability API
  slug: cerner-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-capability-api-openapi.yml
- filename: cerner-condition-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Condition API
  slug: cerner-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-condition-api-openapi.yml
- filename: cerner-definitions-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Definitions API
  slug: cerner-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-definitions-api-openapi.yml
- filename: cerner-encounter-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Encounter API
  slug: cerner-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-encounter-api-openapi.yml
- filename: cerner-generic-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Generic API
  slug: cerner-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-generic-api-openapi.yml
- filename: cerner-patient-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Patient API
  slug: cerner-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-patient-api-openapi.yml
- filename: cerner-procedure-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Procedure API
  slug: cerner-procedure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-procedure-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Cerner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Oracle Health (Cerner) secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Oracle Health (Cerner)
provider_slug: cerner
scheme_count: 1
schemes:
- description: 'SMART on FHIR OAuth 2.0. Every endpoint is tenant-scoped: the tenant id is a path segment of both the FHIR service root and the authorization server, so a client must resolve the tenant before it can authenticate. Public clients use authorization-code with PKCE (S256); confidential clients may use client_secret_basic or private_key_jwt (RS384/ES384). Backend services use client-credentials with system/ scopes and asymmetric client authentication.'
  endpoints:
    introspection_endpoint: https://authorization.cerner.com/tokeninfo
    jwks_uri: https://authorization.cerner.com/jwk
    management_endpoint: https://authorization.cerner.com/tenants/{tenant}/personas/provider/my-authorizations
    revocation_endpoint: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token/revoke
  flows:
  - authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/provider/authorize
    flow: authorizationCode
    scopes: 200
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/hosts/fhir-ehr-code.cerner.com/protocols/oauth2/profiles/smart-v1/token
  - flow: clientCredentials
    scopes: 103
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/hosts/fhir-ehr-code.cerner.com/protocols/oauth2/profiles/smart-v1/token
  issuer: https://authorization.cerner.com/tenants/{tenant}
  name: smartOnFhir
  sources:
  - https://fhir-ehr-code.cerner.com/r4/ec2458f2-1e24-41c8-b71b-0e701af7583d/.well-known/smart-configuration
  - openapi/cerner-millennium-fhir-r4-openapi.yml
  type: oauth2
slug: cerner-authentication
source_filename: cerner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://fhir-ehr-code.cerner.com/r4/ec2458f2-1e24-41c8-b71b-0e701af7583d/.well-known/smart-configuration\ndocs: https://docs.oracle.com/en/industries/health/millennium-platform-apis/mfrap/index.html\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  profile: SMART on FHIR App Launch (SMART v1 and v2)\n  pkce:\n  - S256\n  client_auth_methods:\n  - client_secret_basic\n  - private_key_jwt\n  client_auth_signing_algs:\n  - RS384\n  - ES384\n  scope_count: 303\n  anonymous_surface: The open endpoint https://fhir-open.cerner.com/r4/{tenant} serves read-only data with no token.\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  description: 'SMART on FHIR OAuth 2.0. Every endpoint is tenant-scoped: the tenant id is a path segment of both\n    the FHIR service root and the authorization server, so a client must resolve the tenant before it can authenticate.\n    Public\
  \ clients use authorization-code with PKCE (S256); confidential clients may use client_secret_basic or\n    private_key_jwt (RS384/ES384). Backend services use client-credentials with system/ scopes and asymmetric client\n    authentication.'\n  issuer: https://authorization.cerner.com/tenants/{tenant}\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/provider/authorize\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/hosts/fhir-ehr-code.cerner.com/protocols/oauth2/profiles/smart-v1/token\n    scopes: 200\n  - flow: clientCredentials\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/hosts/fhir-ehr-code.cerner.com/protocols/oauth2/profiles/smart-v1/token\n    scopes: 103\n  endpoints:\n    jwks_uri: https://authorization.cerner.com/jwk\n    introspection_endpoint: https://authorization.cerner.com/tokeninfo\n    revocation_endpoint: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token/revoke\n\
  \    management_endpoint: https://authorization.cerner.com/tenants/{tenant}/personas/provider/my-authorizations\n  sources:\n  - https://fhir-ehr-code.cerner.com/r4/ec2458f2-1e24-41c8-b71b-0e701af7583d/.well-known/smart-configuration\n  - openapi/cerner-millennium-fhir-r4-openapi.yml\ndiscovery:\n  well_known_path: /.well-known/smart-configuration\n  served_at: the FHIR service root, per tenant — not at the host root (the host root returns 502)\n  capability_statement: https://fhir-ehr-code.cerner.com/r4/ec2458f2-1e24-41c8-b71b-0e701af7583d/metadata\n  smart_oauth_uris_extension: http://fhir-registry.smarthealthit.org/StructureDefinition/oauth-uris\nregistration:\n  model: manual — apps are registered in the Oracle Health developer console; there is no dynamic client registration\n    endpoint in the discovery document\n  console: https://www.oracle.com/health/developer/\n  note: code.cerner.com (the former Cerner Code Console) now 301s to https://www.oracle.com/health/developer/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/authentication/cerner-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Bulk FHIR
- CapabilityStatement
- CareAware
- Cerner Millennium
- Clinical Data
- Code Console
- EHR
- Electronic Health Records
- FHIR
- Fortune 1000
- HL7
- HL7v2
- Healthcare
- Interoperability
- Millennium Platform
- Multi-Tenant
- Authentication
- Oracle
- Oracle Health
- Patient Access
- Provider Directory
- SMART Backend Services
- SMART on FHIR
- US Core
---
