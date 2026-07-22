---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fintary.com
  spf: true
hosts:
- cert_expires: Oct 14 22:50:08 2026 GMT
  host: fintary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fintary
provider_slug: fintary
slug: fintary-domain-security
source_filename: fintary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fintary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fintary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/security/fintary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Commissions
- Revenue Operations
- Analytics
---
