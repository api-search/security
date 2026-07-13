---
api_specs:
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Renders API
  slug: renders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
- filename: creatomate-openapi.yml
  format: yaml
  label: Creatomate Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/openapi/creatomate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creatomate.com
  spf: true
hosts:
- cert_expires: Aug 27 12:29:13 2026 GMT
  host: creatomate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 12:29:13 2026 GMT
  host: api.creatomate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creatomate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creatomate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Creatomate
provider_slug: creatomate
slug: creatomate-domain-security
source_filename: creatomate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creatomate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:29:13 2026 GMT\n  hsts: false\n- host: api.creatomate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:29:13 2026 GMT\n  hsts: null\ndomains:\n- domain: creatomate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatomate/refs/heads/main/security/creatomate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Video Generation
- Image Generation
- Automation
- Templates
- Rendering
---
