---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lunarwerx.com
  spf: true
hosts:
- cert_expires: Feb 15 05:44:14 2027 GMT
  host: lunarwerx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LunarWerx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LunarWerx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LunarWerx
provider_slug: lunarwerx-com
slug: lunarwerx-com-domain-security
source_filename: lunarwerx-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunarwerx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 05:44:14 2027 GMT\n  hsts: false\ndomains:\n- domain: lunarwerx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lunarwerx-com/security/lunarwerx-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Desktop Utilities
- Developer Tools
- AI Tooling
- Media Server Tools
- Mobile App
- Software Studio
---
