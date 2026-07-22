---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duke-energy.com
  spf: true
hosts:
- cert_expires: Aug  7 05:59:28 2026 GMT
  host: www.duke-energy.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duke Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for duke-energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: duke-energy
provider_slug: duke-energy
slug: duke-energy-domain-security
source_filename: duke-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duke-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 05:59:28 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: duke-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duke-energy/refs/heads/main/security/duke-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
