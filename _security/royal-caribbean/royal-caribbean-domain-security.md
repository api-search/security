---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: royalcaribbeangroup.com
  spf: false
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.royalcaribbeangroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Royal Caribbean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Royal Caribbean Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Royal Caribbean Group
provider_slug: royal-caribbean
slug: royal-caribbean-domain-security
source_filename: royal-caribbean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.royalcaribbeangroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: royalcaribbeangroup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/royal-caribbean/refs/heads/main/security/royal-caribbean-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cruise Lines
- Travel
- Hospitality
---
