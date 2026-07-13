---
api_specs:
- filename: perses-openapi.yml
  format: yaml
  label: Perses API
  slug: perses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perses/refs/heads/main/openapi/perses-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: perses.dev
  spf: false
hosts:
- cert_expires: Sep 20 13:17:08 2026 GMT
  host: perses.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perses Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perses, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Perses
provider_slug: perses
slug: perses-domain-security
source_filename: perses-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perses.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:17:08 2026 GMT\n  hsts: false\ndomains:\n- domain: perses.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perses/refs/heads/main/security/perses-domain-security.yml
summary_line: TLSv1.3
tags:
- CNCF
- Dashboards
- Monitoring
- Observability
- Open Source
- Time Series
- Visualization
---
