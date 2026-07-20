---
api_specs:
- filename: bcb-group-payments-openapi.json
  format: json
  label: BCB Group Payments API
  slug: bcb-group-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/openapi/bcb-group-payments-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bcbgroup.io
  spf: true
hosts:
- cert_expires: Aug 20 00:21:51 2026 GMT
  host: bcbgroup.io
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bcb Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BCB Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BCB Group
provider_slug: bcb-group
slug: bcb-group-domain-security
source_filename: bcb-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bcbgroup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:21:51 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: bcbgroup.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/security/bcb-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Payments
- Banking
- Digital Assets
- Stablecoins
- Financial Services
- Fintech
---
