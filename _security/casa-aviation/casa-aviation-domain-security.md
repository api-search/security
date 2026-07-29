---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: casa.gov.au
  spf: true
hosts:
- cert_expires: Aug 24 22:18:29 2026 GMT
  host: www.casa.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: my.casa.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: services.casa.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casa Aviation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civil Aviation Safety Authority (CASA), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Civil Aviation Safety Authority (CASA)
provider_slug: casa-aviation
slug: casa-aviation-domain-security
source_filename: casa-aviation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.casa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:18:29 2026 GMT\n  hsts: null\n- host: my.casa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.casa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: casa.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casa-aviation/refs/heads/main/security/casa-aviation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- Aviation
- Airports
- Government
- Regulator
- Aviation Safety
- Open Data
- Drones
---
