---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: propico.in
  spf: true
hosts:
- cert_expires: Oct  2 21:59:39 2026 GMT
  host: propico.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:47:50 2026 GMT
  host: api.propico.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leap To Win Technologies Private Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leap To Win Technologies Private, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leap To Win Technologies Private
provider_slug: leap-to-win-technologies-private
slug: leap-to-win-technologies-private-domain-security
source_filename: leap-to-win-technologies-private-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propico.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.propico.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:47:50 2026 GMT\n  hsts: null\ndomains:\n- domain: propico.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap-to-win-technologies-private/refs/heads/main/security/leap-to-win-technologies-private-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Property Management
- Rental
- Insurance
- India
- Consumer
---
