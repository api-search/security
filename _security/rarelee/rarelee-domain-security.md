---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rarelee.co.kr
  spf: true
hosts:
- cert_expires: Oct 11 10:14:20 2026 GMT
  host: rarelee.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rarelee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RareLee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: RareLee
provider_slug: rarelee
slug: rarelee-domain-security
source_filename: rarelee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rarelee.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:14:20 2026 GMT\n  hsts: false\ndomains:\n- domain: rarelee.co.kr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rarelee/refs/heads/main/security/rarelee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Style Consulting
- Fashion
- Beauty
- Personalization
- Consumer Services
- South Korea
---
