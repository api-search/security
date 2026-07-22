---
api_specs:
- filename: palmetto-energy-intelligence-openapi.json
  format: json
  label: Palmetto Energy Intelligence API
  slug: palmetto-energy-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palmetto/refs/heads/main/openapi/palmetto-energy-intelligence-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: palmetto.com
  spf: true
hosts:
- cert_expires: Oct 12 03:44:03 2026 GMT
  host: palmetto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:44:03 2026 GMT
  host: ei.palmetto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palmetto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palmetto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Palmetto
provider_slug: palmetto
slug: palmetto-domain-security
source_filename: palmetto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palmetto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:44:03 2026 GMT\n  hsts: false\n- host: ei.palmetto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:44:03 2026 GMT\n  hsts: false\ndomains:\n- domain: palmetto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palmetto/refs/heads/main/security/palmetto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Clean Energy
- Solar
- Energy
- Building Energy Modeling
- Home Energy
- Financing
- Sustainability
---
