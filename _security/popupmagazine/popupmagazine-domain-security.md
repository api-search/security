---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: popupmagazine.com
  spf: true
hosts:
- cert_expires: Oct 14 10:13:48 2026 GMT
  host: popupmagazine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popupmagazine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pop-Up Magazine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pop-Up Magazine
provider_slug: popupmagazine
slug: popupmagazine-domain-security
source_filename: popupmagazine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: popupmagazine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: popupmagazine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popupmagazine/refs/heads/main/security/popupmagazine-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Media
- Live Events
- Storytelling
- Publishing
- Entertainment
- Brand Studio
---
