---
api_specs:
- filename: ucd-duchas.yaml
  format: yaml
  label: Dúchas API (National Folklore Collection, UCD)
  slug: duchas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-duchas.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ucd.ie
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.ucd.ie
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: digital.ucd.ie
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Sep  1 12:36:48 2026 GMT
  host: libguides.ucd.ie
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University College Dublin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University College Dublin
provider_slug: ucd
slug: ucd-domain-security
source_filename: ucd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucd.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\n- host: digital.ucd.ie\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: libguides.ucd.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:36:48 2026 GMT\n  hsts: null\ndomains:\n- domain: ucd.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/security/ucd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Ireland
- Library
- Digital Library
- IIIF
- Open Access
- Cultural Heritage
---
