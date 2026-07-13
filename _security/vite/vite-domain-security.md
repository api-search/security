---
api_specs:
- filename: vite-javascript-api-openapi.yml
  format: yaml
  label: Vite JavaScript API
  slug: javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/openapi/vite-javascript-api-openapi.yml
- filename: vite-plugin-api-openapi.yml
  format: yaml
  label: Vite Plugin API
  slug: plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/openapi/vite-plugin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: vitejs.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: vite.dev
  spf: false
hosts:
- cert_expires: Aug 17 21:14:02 2026 GMT
  host: vitejs.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 21:14:02 2026 GMT
  host: vite.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vite, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Vite
provider_slug: vite
slug: vite-domain-security
source_filename: vite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitejs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vitejs.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: vite.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/security/vite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Build Tools
- Bundler
- Development Server
- ESM
- Frontend
- Hot Module Replacement
- JavaScript
- Plugin API
- TypeScript
- Vite
---
