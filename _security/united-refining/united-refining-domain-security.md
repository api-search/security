---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urc.com
  spf: true
hosts:
- cert_expires: Sep  7 13:02:31 2026 GMT
  host: www.urc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: United Refining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Refining Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: United Refining Company
provider_slug: united-refining
slug: united-refining-domain-security
source_filename: united-refining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 13:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-refining/refs/heads/main/security/united-refining-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Petroleum
- Refining
- Fuel
- Retail
- Energy
---
