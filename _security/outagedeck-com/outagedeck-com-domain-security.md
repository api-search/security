---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: outagedeck.com
  spf: true
hosts:
- cert_expires: Feb  4 05:26:41 2027 GMT
  host: outagedeck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OutageDeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OutageDeck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OutageDeck
provider_slug: outagedeck-com
slug: outagedeck-com-domain-security
source_filename: outagedeck-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outagedeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 05:26:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: outagedeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/outagedeck-com/security/outagedeck-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Status
- incident tracking
- Alerts
- Developer Tools
---
