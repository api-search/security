---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zylalabs.com
  spf: true
hosts:
- cert_expires: Aug 25 19:43:25 2026 GMT
  host: zylalabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zyla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zyla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zyla
provider_slug: zyla
slug: zyla-domain-security
source_filename: zyla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zylalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 19:43:25 2026 GMT\n  hsts: null\ndomains:\n- domain: zylalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zyla/refs/heads/main/security/zyla-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Hub
- Discovery
- Marketplace
- Platform
- Search
---
