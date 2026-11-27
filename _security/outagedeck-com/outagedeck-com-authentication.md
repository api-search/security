---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outagedeck-com-badges-api-openapi.yml
  format: yaml
  label: OutageDeck Badges API
  slug: outagedeck-com-badges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-badges-api-openapi.yml
- filename: outagedeck-com-incidents-api-openapi.yml
  format: yaml
  label: OutageDeck Incidents API
  slug: outagedeck-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-incidents-api-openapi.yml
- filename: outagedeck-com-monitoring-api-openapi.yml
  format: yaml
  label: OutageDeck Monitoring API
  slug: outagedeck-com-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-monitoring-api-openapi.yml
- filename: outagedeck-com-providers-api-openapi.yml
  format: yaml
  label: OutageDeck Providers API
  slug: outagedeck-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-providers-api-openapi.yml
- filename: outagedeck-com-services-api-openapi.yml
  format: yaml
  label: OutageDeck Services API
  slug: outagedeck-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-services-api-openapi.yml
- filename: outagedeck-com-status-api-openapi.yml
  format: yaml
  label: OutageDeck Status API
  slug: outagedeck-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outagedeck-com/openapi/outagedeck-com-status-api-openapi.yml
auth_types: []
description: OutageDeck authenticates webhook deliveries using an HMAC signature.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OutageDeck Authentication
name_suffix: Authentication
oauth_flows: []
overview: OutageDeck declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OutageDeck
provider_slug: outagedeck-com
scheme_count: 1
schemes:
- evidence: 'Every generic-webhook delivery carries an OutageDeck-Signature header: t=<unix seconds>,v1=<hex> . The signature is HMAC-SHA256 over <timestamp>:<raw body> using the secret shown once when you created the subscription.'
  header: OutageDeck-Signature
  how_to_obtain: The secret is displayed once on the account page when you create the subscription and can be rotated from the same page.
  location: header
  name: OutageDeck webhook signature
  type: hmac
slug: outagedeck-com-authentication
source_filename: outagedeck-com-authentication.yml
source_heading: Authentication Profile
source_url: https://outagedeck.com/developers/alerts
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://outagedeck.com/developers/alerts\nsources:\n- https://outagedeck.com/developers/alerts\ndescription: OutageDeck authenticates webhook deliveries using an HMAC signature.\nschemes:\n- type: hmac\n  name: OutageDeck webhook signature\n  evidence: 'Every generic-webhook delivery carries an OutageDeck-Signature header: t=<unix seconds>,v1=<hex> . The signature is HMAC-SHA256 over\n    <timestamp>:<raw body> using the secret shown once when you created the subscription.'\n  location: header\n  header: OutageDeck-Signature\n  how_to_obtain: The secret is displayed once on the account page when you create the subscription and can be rotated from the same page.\nnote: No OAuth2, API key, HTTP basic, bearer, JWT, MTLS, or other authentication schemes are documented on the page.\ndocs: https://outagedeck.com/developers/alerts\n"
source_yaml_url: https://artifacts.apis.io/outagedeck-com/authentication/outagedeck-com-authentication.yml
summary_line: 1 scheme
tags:
- Cloud Status
- incident tracking
- Alerts
- Developer Tools
---
