---
api_specs:
- filename: elysiatools-com-openapi-generated.yml
  format: yaml
  label: Elysia Tools API
  slug: elysiatools-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elysiatools-com/openapi/_ae-authored/elysiatools-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elysiatools.com
  spf: true
hosts:
- cert_expires: Dec 10 09:57:56 2026 GMT
  host: elysiatools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elysia Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elysia Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elysia Tools
provider_slug: elysiatools-com
slug: elysiatools-com-domain-security
source_filename: elysiatools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elysiatools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 09:57:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elysiatools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elysiatools-com/security/elysiatools-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tools
- Free
- Online
- Utilities
---
