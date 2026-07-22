---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mathem.se
  spf: true
hosts:
- cert_expires: Aug 24 10:37:56 2026 GMT
  host: www.mathem.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mathem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mathem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mathem
provider_slug: mathem
slug: mathem-domain-security
source_filename: mathem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mathem.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:37:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mathem.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathem/refs/heads/main/security/mathem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Grocery
- E-Commerce
- Retail
- Food Delivery
- Sweden
- Nordics
---
