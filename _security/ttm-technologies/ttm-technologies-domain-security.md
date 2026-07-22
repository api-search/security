---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ttm.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.ttm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ttm Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TTM Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TTM Technologies
provider_slug: ttm-technologies
slug: ttm-technologies-domain-security
source_filename: ttm-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ttm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ttm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ttm-technologies/refs/heads/main/security/ttm-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Contract Manufacturing
- Defense
- Electronics Manufacturing
- Mission Systems
- PCB
- RF and Microwave
- Supply Chain
---
