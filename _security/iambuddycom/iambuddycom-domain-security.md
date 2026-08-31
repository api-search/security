---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buddy.insure
  spf: true
hosts:
- cert_expires: Aug 23 18:43:51 2026 GMT
  host: buddy.insure
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iambuddycom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iambuddy.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iambuddy.com
provider_slug: iambuddycom
slug: iambuddycom-domain-security
source_filename: iambuddycom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buddy.insure\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buddy.insure\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iambuddycom/refs/heads/main/security/iambuddycom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Embedded Insurance
- Insurance Commerce
- P&C Insurance
- MCP
- Payments
---
