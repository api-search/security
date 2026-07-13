---
api_specs:
- filename: national-science-foundation-openapi.yml
  format: yaml
  label: National Science Foundation API
  slug: national-science-foundation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-science-foundation/refs/heads/main/openapi/national-science-foundation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nsf.gov
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.nsf.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.nsf.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: National Science Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Science Foundation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Science Foundation
provider_slug: national-science-foundation
slug: national-science-foundation-domain-security
source_filename: national-science-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nsf.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nsf.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nsf.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-science-foundation/refs/heads/main/security/national-science-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Research
- Science
---
