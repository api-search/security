---
api_specs:
- filename: materials-project-openapi.yml
  format: yaml
  label: Materials Project API
  slug: materials-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-project/refs/heads/main/openapi/materials-project-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: materialsproject.org
  spf: true
hosts:
- cert_expires: Oct  3 14:29:19 2026 GMT
  host: materialsproject.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:29:19 2026 GMT
  host: next-gen.materialsproject.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:29:19 2026 GMT
  host: api.materialsproject.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Materials Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materials Project, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Materials Project
provider_slug: materials-project
slug: materials-project-domain-security
source_filename: materials-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: materialsproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:29:19 2026 GMT\n  hsts: null\n- host: next-gen.materialsproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:29:19 2026 GMT\n  hsts: null\n- host: api.materialsproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:29:19 2026 GMT\n  hsts: null\ndomains:\n- domain: materialsproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materials-project/refs/heads/main/security/materials-project-domain-security.yml
summary_line: TLSv1.3
tags:
- Chemistry
- Materials Science
- Physics
- Research
- Scientific Computing
---
