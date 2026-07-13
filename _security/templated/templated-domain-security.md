---
api_specs:
- filename: templated-openapi.yml
  format: yaml
  label: Templated Render API
  slug: render
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Renders API
  slug: renders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: templated.io
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: templated.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.templated.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Templated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Templated, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Templated
provider_slug: templated
slug: templated-domain-security
source_filename: templated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: templated.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.templated.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: templated.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/security/templated-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Image Generation
- PDF Generation
- Templates
- Rendering
- Automation
---
