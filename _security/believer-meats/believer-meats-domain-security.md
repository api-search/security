---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: believermeats.com
  spf: true
hosts:
- cert_expires: Sep 30 05:13:14 2026 GMT
  host: www.believermeats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Believer Meats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Believer Meats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Believer Meats
provider_slug: believer-meats
slug: believer-meats-domain-security
source_filename: believer-meats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.believermeats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: believermeats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/believer-meats/refs/heads/main/security/believer-meats-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cellular Agriculture
- Cultivated Meat
- Alternative Protein
- Food Technology
- Biotechnology
- Manufacturing
- Defunct
- United States
- Israel
---
