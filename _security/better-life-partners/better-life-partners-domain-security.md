---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: betterlifepartners.com
  spf: true
hosts:
- cert_expires: Oct 25 12:25:14 2026 GMT
  host: betterlifepartners.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Better Life Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Life Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Better Life Partners
provider_slug: better-life-partners
slug: better-life-partners-domain-security
source_filename: better-life-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betterlifepartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:25:14 2026 GMT\n  hsts: false\ndomains:\n- domain: betterlifepartners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-life-partners/refs/heads/main/security/better-life-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Addiction Treatment
- Substance Use Disorder
- Telehealth
- Mental Health
- Value-Based Care
- Health Plans
---
