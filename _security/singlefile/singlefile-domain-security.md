---
api_specs:
- filename: singlefile-openapi.yml
  format: yaml
  label: SingleFile External API
  slug: singlefile-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/openapi/singlefile-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: singlefile.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: singlefile.ai
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.singlefile.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.demo.singlefile.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singlefile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SingleFile, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SingleFile
provider_slug: singlefile
slug: singlefile-domain-security
source_filename: singlefile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.singlefile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: api.demo.singlefile.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: singlefile.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: singlefile.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/security/singlefile-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Compliance
- Legal
- Entity Management
- Corporate Compliance
- Registered Agent
- Business Filings
- Regulatory
- API
- Webhooks
- OAuth
---
