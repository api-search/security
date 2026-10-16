---
api_specs:
- filename: forsakringskassan-rtfkompletteringcontroller-api-openapi.yml
  format: yaml
  label: Försäkringskassan Rtf Komplettering Controller API
  slug: forsakringskassan-rtfkompletteringcontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsakringskassan/refs/heads/main/openapi/forsakringskassan-rtfkompletteringcontroller-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: forsakringskassan.se
  spf: true
hosts:
- cert_expires: Feb 12 13:59:22 2027 GMT
  host: forsakringskassan.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Forsakringskassan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Försäkringskassan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Försäkringskassan
provider_slug: forsakringskassan
slug: forsakringskassan-domain-security
source_filename: forsakringskassan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forsakringskassan.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 13:59:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forsakringskassan.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forsakringskassan/refs/heads/main/security/forsakringskassan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- SocialSecurity
- Sweden
- PublicSector
- API
---
