---
api_specs:
- filename: merlonix-com-alerts-api-openapi.yml
  format: yaml
  label: Merlonix Alerts API
  slug: merlonix-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-alerts-api-openapi.yml
- filename: merlonix-com-assets-api-openapi.yml
  format: yaml
  label: Merlonix Assets API
  slug: merlonix-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-assets-api-openapi.yml
- filename: merlonix-com-channels-api-openapi.yml
  format: yaml
  label: Merlonix Channels API
  slug: merlonix-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-channels-api-openapi.yml
- filename: merlonix-com-checks-api-openapi.yml
  format: yaml
  label: Merlonix Checks API
  slug: merlonix-com-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-checks-api-openapi.yml
- filename: merlonix-com-clients-api-openapi.yml
  format: yaml
  label: Merlonix Clients API
  slug: merlonix-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-clients-api-openapi.yml
- filename: merlonix-com-status-pages-api-openapi.yml
  format: yaml
  label: Merlonix Status pages API
  slug: merlonix-com-status-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merlonix-com/openapi/merlonix-com-status-pages-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: merlonix.com
  spf: true
hosts:
- cert_expires: Jan 16 05:45:27 2027 GMT
  host: merlonix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merlonix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merlonix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Merlonix
provider_slug: merlonix-com
slug: merlonix-com-domain-security
source_filename: merlonix-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merlonix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 05:45:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: merlonix.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/merlonix-com/security/merlonix-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Uptime
- TLS
- DNS
- Alerting
- AI Triage
- Agency Tools
---
