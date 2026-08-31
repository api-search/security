---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carelulu.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: carelulu.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Carelulu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareLuLu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CareLuLu
provider_slug: carelulu
slug: carelulu-domain-security
source_filename: carelulu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carelulu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: carelulu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carelulu/refs/heads/main/security/carelulu-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Child Care
- Daycare
- Preschool
- Marketplace
- Parenting
- Directory
- Reviews
---
