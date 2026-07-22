---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coty.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.coty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coty
provider_slug: coty
slug: coty-domain-security
source_filename: coty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: coty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coty/refs/heads/main/security/coty-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Beauty
- Body Care
- Color Cosmetics
- Consumer Beauty
- Cosmetics
- EDI
- Fortune 500
- Fragrance
- Hair Care
- Licensed Brands
- NYSE
- Personal Care
- Prestige
- Skin Care
- Supplier Portal
---
