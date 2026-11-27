---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kwant.sh
  spf: true
hosts:
- cert_expires: Jan 25 15:56:01 2027 GMT
  host: kwant.sh
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kwant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kwant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kwant
provider_slug: kwant-sh
slug: kwant-sh-domain-security
source_filename: kwant-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kwant.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 15:56:01 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kwant.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kwant-sh/security/kwant-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantitative
- Finance
- Artificial Intelligence
- MCP
- Market Data
---
