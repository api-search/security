---
api_specs:
- filename: socotra-openapi-original.json
  format: json
  label: Socotra Insurance Suite API
  slug: socotra-insurance-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socotra.com
  spf: true
hosts:
- cert_expires: Sep 30 04:15:27 2026 GMT
  host: socotra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 14:50:23 2026 GMT
  host: docs.socotra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 17:40:37 2027 GMT
  host: api.sandbox.socotra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socotra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socotra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Socotra
provider_slug: socotra
slug: socotra-domain-security
source_filename: socotra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socotra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:15:27 2026 GMT\n  hsts: false\n- host: docs.socotra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 14:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sandbox.socotra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 17:40:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socotra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/security/socotra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Core Platform
- Policy Administration
- Billing
- Claims
- Underwriting
- API
- MCP
---
