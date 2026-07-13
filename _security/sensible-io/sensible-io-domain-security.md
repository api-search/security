---
api_specs:
- filename: sensible-io-openapi.yml
  format: yaml
  label: Sensible REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sensible.so
  spf: true
hosts:
- cert_expires: Sep 10 07:22:36 2026 GMT
  host: www.sensible.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:47:53 2026 GMT
  host: docs.sensible.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.sensible.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensible Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensible, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sensible
provider_slug: sensible-io
slug: sensible-io-domain-security
source_filename: sensible-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:22:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:47:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sensible.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/security/sensible-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document AI
- IDP
- Extraction
- LLM
- SenseML
- PDF
---
