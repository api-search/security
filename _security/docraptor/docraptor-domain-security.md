---
api_specs:
- filename: docraptor-openapi.yml
  format: yaml
  label: DocRaptor REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docraptor/refs/heads/main/openapi/docraptor-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docraptor.com
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: docraptor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.docraptor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docraptor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocRaptor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DocRaptor
provider_slug: docraptor
slug: docraptor-domain-security
source_filename: docraptor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docraptor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.docraptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: docraptor.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docraptor/refs/heads/main/security/docraptor-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Document Generation
- PDF
- HTML
- Excel
- API
- Prince
---
