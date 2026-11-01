---
api_specs:
- filename: pluga-actions-api-openapi.yml
  format: yaml
  label: Pluga Actions API
  slug: pluga-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pluga/openapi/pluga-actions-api-openapi.yml
- filename: pluga-basicinfo-api-openapi.yml
  format: yaml
  label: Pluga Basic Info API
  slug: pluga-basicinfo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pluga/openapi/pluga-basicinfo-api-openapi.yml
- filename: pluga-helpers-api-openapi.yml
  format: yaml
  label: Pluga Helpers API
  slug: pluga-helpers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pluga/openapi/pluga-helpers-api-openapi.yml
- filename: pluga-triggers-api-openapi.yml
  format: yaml
  label: Pluga Triggers API
  slug: pluga-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pluga/openapi/pluga-triggers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pluga.co
  spf: true
hosts:
- cert_expires: Dec  7 18:23:10 2026 GMT
  host: pluga.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pluga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pluga
provider_slug: pluga
slug: pluga-domain-security
source_filename: pluga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluga.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 18:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pluga.co\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pluga/security/pluga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automation
- Integration
- No-Code
- Brazil
---
