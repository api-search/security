---
api_specs:
- filename: elsevier-openapi.yml
  format: yaml
  label: Elsevier Scopus APIs
  slug: elsevier-scopus-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elsevier.com
  spf: true
hosts:
- cert_expires: Nov 15 15:11:04 2026 GMT
  host: dev.elsevier.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 15 15:11:04 2026 GMT
  host: api.elsevier.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elsevier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elsevier, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elsevier
provider_slug: elsevier
slug: elsevier-domain-security
source_filename: elsevier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.elsevier.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 15:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.elsevier.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 15:11:04 2026 GMT\n  hsts: null\ndomains:\n- domain: elsevier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/security/elsevier-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Content
- Journals
- Medical
- Research
- Scientific
- Technical
---
