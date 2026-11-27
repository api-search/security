---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vpndetection-io-account-api-openapi.yml
  format: yaml
  label: VPNDetection Account API
  slug: vpndetection-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-account-api-openapi.yml
- filename: vpndetection-io-api-keys-api-openapi.yml
  format: yaml
  label: VPNDetection API keys API
  slug: vpndetection-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-api-keys-api-openapi.yml
- filename: vpndetection-io-authorization-api-openapi.yml
  format: yaml
  label: VPNDetection Authorization API
  slug: vpndetection-io-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-authorization-api-openapi.yml
- filename: vpndetection-io-database-api-openapi.yml
  format: yaml
  label: VPNDetection Database API
  slug: vpndetection-io-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-database-api-openapi.yml
- filename: vpndetection-io-entitlement-api-openapi.yml
  format: yaml
  label: VPNDetection Entitlement API
  slug: vpndetection-io-entitlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-entitlement-api-openapi.yml
- filename: vpndetection-io-lookup-api-openapi.yml
  format: yaml
  label: VPNDetection Lookup API
  slug: vpndetection-io-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-lookup-api-openapi.yml
- filename: vpndetection-io-organization-api-openapi.yml
  format: yaml
  label: VPNDetection Organization API
  slug: vpndetection-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-organization-api-openapi.yml
auth_types: []
description: Authentication schemes used by the VPNDetection API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: VPNDetection Authentication
name_suffix: Authentication
oauth_flows: []
overview: VPNDetection declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: VPNDetection
provider_slug: vpndetection-io
scheme_count: 1
schemes:
- evidence: 'Any one of:


    - bearer token (scopes: apikeys.manage)'
  header: Authorization
  location: header
  name: Bearer
  scopes:
  - apikeys.manage
  - apikeys.read
  - apikeys.reveal
  type: http-bearer
slug: vpndetection-io-authentication
source_filename: vpndetection-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.vpndetection.io/api/api-keys/accountCreateApikey.mdx
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.vpndetection.io/api/api-keys/accountCreateApikey.mdx\nsources:\n- https://docs.vpndetection.io/api/api-keys/accountCreateApikey.mdx\n- https://docs.vpndetection.io/api/api-keys/accountListApikeys.mdx\n- https://docs.vpndetection.io/api/api-keys/accountRevealApikey.mdx\n- https://docs.vpndetection.io/api/api-keys/accountRevokeApikey.mdx\ndescription: Authentication schemes used by the VPNDetection API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Any one of:\n\n\n    - bearer token (scopes: apikeys.manage)'\n  location: header\n  header: Authorization\n  scopes:\n  - apikeys.manage\n  - apikeys.read\n  - apikeys.reveal\nnote: No OAuth flows, token URLs, or authorization URLs are documented.\ndocs: https://docs.vpndetection.io/api/api-keys/accountCreateApikey.mdx\n"
source_yaml_url: https://artifacts.apis.io/vpndetection-io/authentication/vpndetection-io-authentication.yml
summary_line: 1 scheme
tags:
- VPN
- IP
- Security
- Data
- Detection
---
