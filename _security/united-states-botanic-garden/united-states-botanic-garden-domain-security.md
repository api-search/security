---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: usbg.gov
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.usbg.gov
  hsts: true
  hsts_max_age: 8035200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States Botanic Garden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Botanic Garden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: United States Botanic Garden
provider_slug: united-states-botanic-garden
slug: united-states-botanic-garden-domain-security
source_filename: united-states-botanic-garden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usbg.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 8035200\ndomains:\n- domain: usbg.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-botanic-garden/refs/heads/main/security/united-states-botanic-garden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Federal Government
- Botany
- Plants
- Conservation
- Education
---
