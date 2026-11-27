---
api_specs:
- filename: usero-io-openapi-generated.yml
  format: yaml
  label: Usero API
  slug: usero-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usero-io/openapi/_ae-authored/usero-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usero.io
  spf: true
hosts:
- cert_expires: Feb 22 12:13:54 2027 GMT
  host: usero.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Usero
provider_slug: usero-io
slug: usero-io-domain-security
source_filename: usero-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 12:13:54 2027 GMT\n  hsts: false\ndomains:\n- domain: usero.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usero-io/security/usero-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Feedback
- Session Replay
- B2B SaaS
---
