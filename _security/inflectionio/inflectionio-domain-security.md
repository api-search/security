---
api_specs:
- filename: inflectionio-openapi-original.yml
  format: yaml
  label: Inflection Developer API
  slug: inflectionio-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inflection.io
  spf: true
hosts:
- cert_expires: Sep 13 20:35:58 2026 GMT
  host: www.inflection.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.inflection.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Inflectionio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflection.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inflection.io
provider_slug: inflectionio
slug: inflectionio-domain-security
source_filename: inflectionio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inflection.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:35:58 2026 GMT\n  hsts: false\n- host: api.inflection.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: inflection.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/security/inflectionio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Saas
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- API
---
