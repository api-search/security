---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marker.page
  spf: true
hosts:
- cert_expires: Oct 18 16:51:00 2026 GMT
  host: marker.page
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marker
provider_slug: marker
slug: marker-domain-security
source_filename: marker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marker.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 16:51:00 2026 GMT\n  hsts: false\ndomains:\n- domain: marker.page\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marker/refs/heads/main/security/marker-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Future Of Work
- Writing
- Productivity
- Text Editor
- Web App
---
