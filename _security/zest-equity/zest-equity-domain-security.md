---
api_specs:
- filename: zest-equity-openapi-original.json
  format: json
  label: Zest Public API
  slug: zest-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zest-equity/refs/heads/main/openapi/zest-equity-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zestequity.com
  spf: true
hosts:
- cert_expires: Oct 13 11:02:28 2026 GMT
  host: zestequity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zest Equity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zest Equity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zest Equity
provider_slug: zest-equity
slug: zest-equity-domain-security
source_filename: zest-equity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zestequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zestequity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zest-equity/refs/heads/main/security/zest-equity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Private Markets
- SPV
- Investments
- Escrow
- Fund Administration
- MENA
- Webhooks
- Regulated
---
