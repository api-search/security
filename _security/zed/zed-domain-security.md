---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zed.co
  spf: true
hosts:
- cert_expires: Oct  1 18:44:48 2026 GMT
  host: www.zed.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zed
provider_slug: zed
slug: zed-domain-security
source_filename: zed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zed.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:44:48 2026 GMT\n  hsts: false\ndomains:\n- domain: zed.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zed/refs/heads/main/security/zed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Credit Cards
- Payments
- Mastercard
- Consumer Finance
- Virtual Cards
- Mobile Banking
- Philippines
- Southeast Asia
---
