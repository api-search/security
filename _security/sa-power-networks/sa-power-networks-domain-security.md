---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sapowernetworks.com.au
  spf: true
hosts:
- cert_expires: Oct  6 10:45:34 2026 GMT
  host: www.sapowernetworks.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: dapr.sapowernetworks.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sa Power Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SA Power Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SA Power Networks
provider_slug: sa-power-networks
slug: sa-power-networks-domain-security
source_filename: sa-power-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sapowernetworks.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:45:34 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: dapr.sapowernetworks.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sapowernetworks.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sa-power-networks/refs/heads/main/security/sa-power-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Smart Metering
- Solar
- DER
- Open Data
---
