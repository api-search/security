---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: riksbank.se
  spf: true
hosts:
- cert_expires: Jan  4 16:01:15 2027 GMT
  host: riksbank.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Riksbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riksbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Riksbank
provider_slug: riksbank
slug: riksbank-domain-security
source_filename: riksbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riksbank.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 16:01:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: riksbank.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riksbank/refs/heads/main/security/riksbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- CentralBank
- Sweden
- Economics
- API
---
