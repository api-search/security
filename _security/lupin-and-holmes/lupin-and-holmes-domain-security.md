---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: landh.tech
  spf: true
hosts:
- cert_expires: Oct 16 03:51:44 2026 GMT
  host: landh.tech
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lupin And Holmes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lupin & Holmes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lupin & Holmes
provider_slug: lupin-and-holmes
slug: lupin-and-holmes-domain-security
source_filename: lupin-and-holmes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landh.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:51:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: landh.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lupin-and-holmes/refs/heads/main/security/lupin-and-holmes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Security
- Offensive Security
- Supply Chain Security
- Vulnerability Management
- Social Engineering
- Security Research
---
