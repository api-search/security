---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sunoco.com
  spf: true
hosts:
- cert_expires: Feb  1 16:33:41 2027 GMT
  host: www.sunoco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunoco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunoco LP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sunoco LP
provider_slug: sunoco
slug: sunoco-domain-security
source_filename: sunoco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunoco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 16:33:41 2027 GMT\n  hsts: null\ndomains:\n- domain: sunoco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunoco/refs/heads/main/security/sunoco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Fuels
- Fuel Distribution
- Convenience Stores
- Midstream
- Pipelines
- Terminals
- Retail
---
