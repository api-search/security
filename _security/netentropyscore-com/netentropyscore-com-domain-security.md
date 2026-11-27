---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netentropyscore.com
  spf: false
hosts:
- cert_expires: Feb  8 08:14:35 2027 GMT
  host: netentropyscore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Net Entropy Score Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Net Entropy Score, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Net Entropy Score
provider_slug: netentropyscore-com
slug: netentropyscore-com-domain-security
source_filename: netentropyscore-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netentropyscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 08:14:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netentropyscore.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/netentropyscore-com/security/netentropyscore-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brands
- Consistency
- Analytics
- Software-as-a-Service
- Marketing
---
