---
api_specs:
- filename: embat-openapi-original.json
  format: json
  label: Embat API
  slug: embat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/embat/refs/heads/main/openapi/embat-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: embat.io
  spf: true
hosts:
- cert_expires: Aug 28 11:25:30 2026 GMT
  host: www.embat.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Embat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Embat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Embat
provider_slug: embat
slug: embat-domain-security
source_filename: embat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.embat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:25:30 2026 GMT\n  hsts: false\ndomains:\n- domain: embat.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embat/refs/heads/main/security/embat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Treasury Management
- Payments
- Cash Flow
- Banking
- Reconciliation
- Forecasting
---
