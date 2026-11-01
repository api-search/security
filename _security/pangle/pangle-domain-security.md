---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pangleglobal.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: pangleglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pangle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pangle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pangle
provider_slug: pangle
slug: pangle-domain-security
source_filename: pangle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pangleglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pangleglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pangle/security/pangle-domain-security.yml
summary_line: TLSv1.3
tags:
- Advertising
- Mobile
- Monetization
- TikTok
- In‑App
---
