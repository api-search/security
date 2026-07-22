---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plink.ai
  spf: true
hosts:
- cert_expires: Oct  1 18:14:27 2026 GMT
  host: www.plink.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plink
provider_slug: plink
slug: plink-domain-security
source_filename: plink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plink.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:14:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plink.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plink/refs/heads/main/security/plink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Card Linking
- Personalization
- Commerce
- Rewards
- Banking
- Fintech
---
