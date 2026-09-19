---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arm.co.za
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: arm.co.za
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Africanrainbowminerals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for African Rainbow Minerals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: African Rainbow Minerals
provider_slug: africanrainbowminerals
slug: africanrainbowminerals-domain-security
source_filename: africanrainbowminerals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arm.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arm.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/africanrainbowminerals/refs/heads/main/security/africanrainbowminerals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Metals And Mining
- Natural Resources
- Commodities
- Iron Ore
- Manganese
- Platinum Group Metals
- Coal
- South Africa
- Publicly Traded
---
