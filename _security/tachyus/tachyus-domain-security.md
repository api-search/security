---
api_specs:
- filename: tachyus-tachapps-openapi.yml
  format: yaml
  label: Tachapps API
  slug: tachapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/openapi/tachyus-tachapps-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tachyus.com
  spf: true
hosts:
- cert_expires: Oct 10 22:51:05 2026 GMT
  host: tachyus.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tachyus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tachyus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tachyus
provider_slug: tachyus
slug: tachyus-domain-security
source_filename: tachyus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tachyus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:51:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: tachyus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/security/tachyus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Reservoir Management
- Production Optimization
- Emissions Management
- Machine Learning
- Analytics
---
