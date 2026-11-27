---
api_specs:
- filename: pagelive-io-openapi-generated.yml
  format: yaml
  label: Pagelive API
  slug: pagelive-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelive-io/openapi/_ae-authored/pagelive-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagelive.io
  spf: true
hosts:
- cert_expires: Feb 16 04:11:28 2027 GMT
  host: pagelive.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pagelive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagelive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pagelive
provider_slug: pagelive-io
slug: pagelive-io-domain-security
source_filename: pagelive-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagelive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 04:11:28 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: pagelive.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pagelive-io/security/pagelive-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Document Sharing
- Secure Links
- Software-as-a-Service
- Collaboration
---
