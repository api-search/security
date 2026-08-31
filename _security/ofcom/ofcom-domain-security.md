---
api_specs:
- filename: ofcom-coverage-api-openapi.yml
  format: yaml
  label: Ofcom Coverage API
  slug: ofcom-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofcom/refs/heads/main/openapi/ofcom-coverage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ofcom.org.uk
  spf: true
hosts:
- cert_expires: Oct 18 09:16:02 2026 GMT
  host: www.ofcom.org.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.ofcom.org.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api-proxy.ofcom.org.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ofcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ofcom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ofcom
provider_slug: ofcom
slug: ofcom-domain-security
source_filename: ofcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ofcom.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 09:16:02 2026 GMT\n  hsts: null\n- host: api.ofcom.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-proxy.ofcom.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ofcom.org.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofcom/refs/heads/main/security/ofcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United Kingdom
- Regulator
- Broadband
- Mobile Network Coverage
- Spectrum
- Open Data
- Connected Nations
---
