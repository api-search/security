---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bureau.id
  spf: true
hosts:
- cert_expires: Dec  4 15:01:55 2026 GMT
  host: bureau.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bureau
provider_slug: bureau
slug: bureau-domain-security
source_filename: bureau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bureau.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 15:01:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bureau.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau/refs/heads/main/security/bureau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Identity Verification
- KYC
- AML
- Fintech
---
