---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yesenergy.com
  spf: true
hosts:
- cert_expires: Sep 28 05:02:21 2026 GMT
  host: www.yesenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: services.yesenergy.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yes Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yes Energy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yes Energy
provider_slug: yes-energy
slug: yes-energy-domain-security
source_filename: yes-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yesenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.yesenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: yesenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yes-energy/refs/heads/main/security/yes-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- Market Data
- Wholesale Power
- ISO RTO
- Renewables
- Trading
---
