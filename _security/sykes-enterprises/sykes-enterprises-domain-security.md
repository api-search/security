---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sykes.com
  spf: true
hosts:
- cert_expires: Oct  3 04:25:52 2026 GMT
  host: www.sykes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.sykes.com
  https: false
- host: api.sykes.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sykes Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sykes Enterprises, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sykes Enterprises
provider_slug: sykes-enterprises
slug: sykes-enterprises-domain-security
source_filename: sykes-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sykes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.sykes.com\n  https: false\n- host: api.sykes.com\n  https: false\ndomains:\n- domain: sykes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sykes-enterprises/refs/heads/main/security/sykes-enterprises-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPO
- Customer Engagement
- Technology
---
