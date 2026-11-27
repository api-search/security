---
api_specs:
- filename: htmldrop-app-openapi-generated.yml
  format: yaml
  label: htmldrop API
  slug: htmldrop-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htmldrop-app/openapi/_ae-authored/htmldrop-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: htmldrop.app
  spf: false
hosts:
- cert_expires: Feb  3 15:19:45 2027 GMT
  host: htmldrop.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: htmldrop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for htmldrop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: htmldrop
provider_slug: htmldrop-app
slug: htmldrop-app-domain-security
source_filename: htmldrop-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: htmldrop.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 15:19:45 2027 GMT\n  hsts: false\ndomains:\n- domain: htmldrop.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/htmldrop-app/security/htmldrop-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- File Hosting
- HTML
- Markdown
- URL Shorteners
- Developer Tools
---
