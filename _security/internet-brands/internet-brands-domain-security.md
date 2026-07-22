---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: internetbrands.com
  spf: true
hosts:
- cert_expires: Aug 22 01:13:25 2026 GMT
  host: www.internetbrands.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Internet Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internet Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Internet Brands
provider_slug: internet-brands
slug: internet-brands-domain-security
source_filename: internet-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.internetbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: internetbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-brands/refs/heads/main/security/internet-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Media
- Health
- Legal
- Dental
- Automotive
- SaaS
- Holding Company
---
