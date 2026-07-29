---
api_specs:
- filename: uk-caa-consultations-api-openapi.yml
  format: yaml
  label: CAA Consultations API
  slug: caa-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-caa/refs/heads/main/openapi/uk-caa-consultations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caa.co.uk
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.caa.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: portal.caa.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:06:42 2026 GMT
  host: consultations.caa.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uk Caa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UK Civil Aviation Authority, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UK Civil Aviation Authority
provider_slug: uk-caa
slug: uk-caa-domain-security
source_filename: uk-caa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caa.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.caa.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\n- host: consultations.caa.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caa.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-caa/refs/heads/main/security/uk-caa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Airports
- Regulator
- Government
- Distribution
- Consumer Protection
- Open Data
---
