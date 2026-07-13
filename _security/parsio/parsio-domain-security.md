---
api_specs:
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Mailboxes API
  slug: parsio-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Documents API
  slug: parsio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Webhooks API
  slug: parsio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parsio.io
  spf: true
hosts:
- cert_expires: Sep 29 03:49:53 2026 GMT
  host: parsio.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 06:57:54 2026 GMT
  host: help.parsio.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:14:46 2026 GMT
  host: api.parsio.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parsio
provider_slug: parsio
slug: parsio-domain-security
source_filename: parsio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parsio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:49:53 2026 GMT\n  hsts: false\n- host: help.parsio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 06:57:54 2026 GMT\n  hsts: false\n- host: api.parsio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:14:46 2026 GMT\n  hsts: null\ndomains:\n- domain: parsio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/security/parsio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Document Parsing
- Email Parsing
- OCR
- Data Extraction
---
