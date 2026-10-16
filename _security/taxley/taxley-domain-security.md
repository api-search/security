---
api_specs:
- filename: taxley-tools-api-openapi.yml
  format: yaml
  label: Taxley (UK Corporation Tax API) Tools API
  slug: taxley-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxley/refs/heads/main/openapi/taxley-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taxley.co.uk
  spf: true
hosts:
- cert_expires: Jan  8 01:20:39 2027 GMT
  host: taxley.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taxley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taxley (UK Corporation Tax API), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taxley (UK Corporation Tax API)
provider_slug: taxley
slug: taxley-domain-security
source_filename: taxley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taxley.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 01:20:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taxley.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxley/refs/heads/main/security/taxley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- UK
- Finance
- API
---
