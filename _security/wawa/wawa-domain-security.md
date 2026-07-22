---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wawa.com
  spf: true
hosts:
- cert_expires: Sep 15 15:07:45 2026 GMT
  host: www.wawa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wawa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wawa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wawa
provider_slug: wawa
slug: wawa-domain-security
source_filename: wawa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wawa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:07:45 2026 GMT\n  hsts: null\ndomains:\n- domain: wawa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wawa/refs/heads/main/security/wawa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Convenience Store
- Fuel Retail
- Food Service
- Loyalty
- Mobile Ordering
- Private Company
- Regional Retail
---
