---
api_specs:
- filename: ubicquia-config-api-openapi-original.json
  format: json
  label: Ubicquia Config API
  slug: ubicquia-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-config-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ubicquia.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.ubicquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: config.api.ubicquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubicquia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubicquia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ubicquia
provider_slug: ubicquia
slug: ubicquia-domain-security
source_filename: ubicquia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubicquia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: config.api.ubicquia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ubicquia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/security/ubicquia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Cities
- Internet of Things
- Energy
- Utilities
- Electric Grid
- Streetlights
- Public Safety
- Infrastructure
- Sensors
- Edge AI
- Transformer Monitoring
---
