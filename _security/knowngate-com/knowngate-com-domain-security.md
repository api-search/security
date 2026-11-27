---
api_specs:
- filename: knowngate-com-openapi-generated.yml
  format: yaml
  label: KnownGate API
  slug: knowngate-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowngate-com/openapi/_ae-authored/knowngate-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: knowngate.com
  spf: false
hosts:
- cert_expires: Jan 30 01:40:32 2027 GMT
  host: knowngate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KnownGate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KnownGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: KnownGate
provider_slug: knowngate-com
slug: knowngate-com-domain-security
source_filename: knowngate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knowngate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 01:40:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: knowngate.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/knowngate-com/security/knowngate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Food
- Artificial Intelligence
- Health
- Free
---
