---
api_specs:
- filename: trymaven-com-health-api-openapi.yml
  format: yaml
  label: Maven Health API
  slug: trymaven-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-health-api-openapi.yml
- filename: trymaven-com-public-api-v1-api-openapi.yml
  format: yaml
  label: Maven Public API (v1) API
  slug: trymaven-com-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-public-api-v1-api-openapi.yml
- filename: trymaven-com-retell-api-openapi.yml
  format: yaml
  label: Maven Retell API
  slug: trymaven-com-retell-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-retell-api-openapi.yml
- filename: trymaven-com-vapi-api-openapi.yml
  format: yaml
  label: Maven VAPI API
  slug: trymaven-com-vapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-vapi-api-openapi.yml
- filename: trymaven-com-widget-sessions-api-openapi.yml
  format: yaml
  label: Maven Widget Sessions API
  slug: trymaven-com-widget-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-widget-sessions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trymaven.com
  spf: false
hosts:
- cert_expires: Dec 22 19:23:18 2026 GMT
  host: trymaven.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trymaven Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Maven
provider_slug: trymaven-com
slug: trymaven-com-domain-security
source_filename: trymaven-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trymaven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 19:23:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trymaven.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/trymaven-com/security/trymaven-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Voice AI
- Chatbots
- API
- FinTech
- Y-Combinator
---
