---
api_specs:
- filename: pixepi-apps-api-openapi.yml
  format: yaml
  label: Pixepi Apps API
  slug: pixepi-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixepi/refs/heads/main/openapi/pixepi-apps-api-openapi.yml
- filename: pixepi-jobs-api-openapi.yml
  format: yaml
  label: Pixepi Jobs API
  slug: pixepi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixepi/refs/heads/main/openapi/pixepi-jobs-api-openapi.yml
- filename: pixepi-usage-api-openapi.yml
  format: yaml
  label: Pixepi Usage API
  slug: pixepi-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixepi/refs/heads/main/openapi/pixepi-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pixepi.com
  spf: true
hosts:
- cert_expires: Dec 21 12:30:50 2026 GMT
  host: pixepi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pixepi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixepi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pixepi
provider_slug: pixepi
slug: pixepi-domain-security
source_filename: pixepi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixepi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: pixepi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixepi/refs/heads/main/security/pixepi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tools
- PDF
- Image
---
