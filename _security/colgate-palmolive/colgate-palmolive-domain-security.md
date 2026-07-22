---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: colgatepalmolive.com
  spf: true
hosts:
- cert_expires: Oct  4 12:03:10 2026 GMT
  host: www.colgatepalmolive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colgate Palmolive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colgate-Palmolive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Colgate-Palmolive
provider_slug: colgate-palmolive
slug: colgate-palmolive-domain-security
source_filename: colgate-palmolive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colgatepalmolive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:03:10 2026 GMT\n  hsts: null\ndomains:\n- domain: colgatepalmolive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colgate-palmolive/refs/heads/main/security/colgate-palmolive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consumer Products
- CPG
- EDI
- Home Care
- Oral Care
- Personal Care
- Pet Nutrition
- Retail
- Fortune 500
---
