---
api_specs:
- filename: dochost-io-openapi-generated.yml
  format: yaml
  label: dochost API
  slug: dochost-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dochost-io/openapi/_ae-authored/dochost-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dochost.io
  spf: true
hosts:
- cert_expires: Dec 28 04:45:40 2026 GMT
  host: dochost.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dochost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dochost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dochost
provider_slug: dochost-io
slug: dochost-io-domain-security
source_filename: dochost-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dochost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:45:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dochost.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dochost-io/security/dochost-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- HTML
- Markdown
- Free
- URLs
---
