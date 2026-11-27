---
anonymous_access: false
api_key_in: []
api_specs:
- filename: domainlab-app-account-api-openapi.yml
  format: yaml
  label: Domain Lab Account API
  slug: domainlab-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-account-api-openapi.yml
- filename: domainlab-app-alerts-api-openapi.yml
  format: yaml
  label: Domain Lab Alerts API
  slug: domainlab-app-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-alerts-api-openapi.yml
- filename: domainlab-app-domain-status-api-openapi.yml
  format: yaml
  label: Domain Lab Domain Status API
  slug: domainlab-app-domain-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-domain-status-api-openapi.yml
- filename: domainlab-app-domains-api-openapi.yml
  format: yaml
  label: Domain Lab Domains API
  slug: domainlab-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-domains-api-openapi.yml
- filename: domainlab-app-email-api-openapi.yml
  format: yaml
  label: Domain Lab Email API
  slug: domainlab-app-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-email-api-openapi.yml
- filename: domainlab-app-event-types-api-openapi.yml
  format: yaml
  label: Domain Lab Event Types API
  slug: domainlab-app-event-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-event-types-api-openapi.yml
- filename: domainlab-app-events-api-openapi.yml
  format: yaml
  label: Domain Lab Events API
  slug: domainlab-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-events-api-openapi.yml
- filename: domainlab-app-inbox-api-openapi.yml
  format: yaml
  label: Domain Lab Inbox API
  slug: domainlab-app-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-inbox-api-openapi.yml
- filename: domainlab-app-notification-rules-api-openapi.yml
  format: yaml
  label: Domain Lab Notification Rules API
  slug: domainlab-app-notification-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-notification-rules-api-openapi.yml
- filename: domainlab-app-registrar-connections-api-openapi.yml
  format: yaml
  label: Domain Lab Registrar Connections API
  slug: domainlab-app-registrar-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-registrar-connections-api-openapi.yml
auth_types: []
description: Authentication methods as published on Domain Lab pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Domain Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Domain Lab declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Domain Lab
provider_slug: domainlab-app
scheme_count: 1
schemes:
- evidence: Every request is authenticated with a Bearer header.
  header: Authorization
  how_to_obtain: Create an API key in Preferences → API; the key starts with dlb_ and is shown once.
  location: header
  name: Bearer
  type: http-bearer
slug: domainlab-app-authentication
source_filename: domainlab-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.domainlab.app/tools/email-auth
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.domainlab.app/tools/email-auth\nsources:\n- https://www.domainlab.app/tools/email-auth\n- https://www.domainlab.app/help/articles/quick-start\n- https://www.domainlab.app/help/articles/api-quick-start\ndescription: Authentication methods as published on Domain Lab pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every request is authenticated with a Bearer header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Preferences → API; the key starts with dlb_ and is shown once.\ndocs: https://www.domainlab.app/tools/email-auth\n"
source_yaml_url: https://artifacts.apis.io/domainlab-app/authentication/domainlab-app-authentication.yml
summary_line: 1 scheme
tags:
- Domain Monitoring
- DNS Monitoring
- SSL Monitoring
- AI Alerts
- Automation Integration
- Webhook Notifications
---
