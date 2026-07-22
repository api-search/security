---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trustingsocial.com
  spf: true
hosts:
- cert_expires: Jan 23 07:41:23 2027 GMT
  host: trustingsocial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TrustIQ
provider_slug: trustiq
slug: trustiq-domain-security
source_filename: trustiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustingsocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 07:41:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trustingsocial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustiq/refs/heads/main/security/trustiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Credit Scoring
- Fraud Detection
- Identity Verification
- Artificial Intelligence
- Financial Services
- Emerging Markets
- Alternative Data
---
