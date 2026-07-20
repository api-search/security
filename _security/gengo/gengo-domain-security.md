---
api_specs:
- filename: gengo-openapi.yml
  format: yaml
  label: Gengo API
  slug: gengo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gengo/refs/heads/main/openapi/gengo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gengo.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: gengo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.gengo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.sandbox.gengo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gengo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gengo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gengo
provider_slug: gengo
slug: gengo-domain-security
source_filename: gengo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.gengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.sandbox.gengo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gengo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gengo/refs/heads/main/security/gengo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Translation
- Localization
- Human Translation
- Language Services
- Internationalization
- Content
- Text
---
