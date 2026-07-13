---
api_specs:
- filename: scispot-openapi.yml
  format: yaml
  label: Scispot API
  slug: scispot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-openapi.yml
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: false
  dnssec: true
  domain: scispot.com
  spf: false
hosts:
- cert_expires: Oct  7 10:52:23 2026 GMT
  host: www.scispot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.scispot.com
  https: false
kind: domain-security
layout: security
method: probed
name: Scispot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scispot, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Scispot
provider_slug: scispot
slug: scispot-domain-security
source_filename: scispot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scispot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:52:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.scispot.com\n  https: false\ndomains:\n- domain: scispot.com\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/security/scispot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Laboratory
- Life Science
- LIMS
- ELN
- Biotech
- API First
- Scientific Data
- Healthcare
---
