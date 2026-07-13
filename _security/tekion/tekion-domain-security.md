---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tekion.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tekioncloud.com
  spf: false
hosts:
- cert_expires: Dec 16 12:21:36 2026 GMT
  host: tekion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: apc.tekioncloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api.tekioncloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tekion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tekion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tekion
provider_slug: tekion
slug: tekion-domain-security
source_filename: tekion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tekion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 12:21:36 2026 GMT\n  hsts: false\n- host: apc.tekioncloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.tekioncloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tekion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tekioncloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekion/refs/heads/main/security/tekion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Dealership
- DMS
- Automotive Retail Cloud
- Partner API
- Sales
- Service
- Inventory
- Parts
- Webhooks
- Gated
---
