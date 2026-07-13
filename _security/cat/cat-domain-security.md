---
api_specs:
- filename: cat-openapi.yml
  format: yaml
  label: CAT Digital Marketplace API
  slug: cat-digital-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cat/refs/heads/main/openapi/cat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cat.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: digital.cat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 23 23:59:59 2026 GMT
  host: www.cat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: services.cat.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CAT
provider_slug: cat
slug: cat-domain-security
source_filename: cat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.cat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 23 23:59:59 2026 GMT\n  hsts: null\n- host: services.cat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cat/refs/heads/main/security/cat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Engines
- Equipment
- Heavy Equipment
- Locomotives
- Manufacturing
- Mining
- Telematics
---
