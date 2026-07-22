---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: incredible.inc
  spf: true
hosts:
- cert_expires: Aug 25 22:20:20 2026 GMT
  host: incredible.inc
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Increbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IncreBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: IncreBio
provider_slug: increbio
slug: increbio-domain-security
source_filename: increbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incredible.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:20:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: incredible.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increbio/refs/heads/main/security/increbio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Food
- Beverage
- Biotech
- Health
- Sugar Reduction
- Consumer Packaged Goods
- Thailand
---
