---
api_specs:
- filename: datavessel-io-openapi-generated.yml
  format: yaml
  label: datavessel API
  slug: datavessel-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datavessel-io/openapi/_ae-authored/datavessel-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datavessel.io
  spf: true
hosts:
- cert_expires: Jan  1 03:12:06 2027 GMT
  host: datavessel.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: datavessel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for datavessel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: datavessel
provider_slug: datavessel-io
slug: datavessel-io-domain-security
source_filename: datavessel-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datavessel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 03:12:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datavessel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datavessel-io/security/datavessel-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Artificial Intelligence
- Automation
- Integration
- MCP
---
