---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: zaver.com
  spf: true
hosts:
- cert_expires: Nov 23 00:49:25 2026 GMT
  host: zaver.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zaver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zaver, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Zaver
provider_slug: zaver
slug: zaver-domain-security
source_filename: zaver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zaver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 00:49:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zaver.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zaver/refs/heads/main/security/zaver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Payments
- Fintech
- E-Commerce
- Software-as-a-Service
- Company
---
