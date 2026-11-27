---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: domainlab.app
  spf: true
hosts:
- cert_expires: Dec 26 22:50:30 2026 GMT
  host: domainlab.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domain Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domain Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Domain Lab
provider_slug: domainlab-app
slug: domainlab-app-domain-security
source_filename: domainlab-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainlab.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 22:50:30 2026 GMT\n  hsts: false\ndomains:\n- domain: domainlab.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domainlab-app/security/domainlab-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Domain Monitoring
- DNS Monitoring
- SSL Monitoring
- AI Alerts
- Automation Integration
- Webhook Notifications
---
