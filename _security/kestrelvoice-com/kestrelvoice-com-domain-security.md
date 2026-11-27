---
api_specs:
- filename: kestrelvoice-com-openapi-generated.yml
  format: yaml
  label: KestrelVoice API
  slug: kestrelvoice-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kestrelvoice-com/openapi/_ae-authored/kestrelvoice-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kestrelvoice.com
  spf: false
hosts:
- cert_expires: Jan 28 06:45:29 2027 GMT
  host: kestrelvoice.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KestrelVoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KestrelVoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: KestrelVoice
provider_slug: kestrelvoice-com
slug: kestrelvoice-com-domain-security
source_filename: kestrelvoice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kestrelvoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 06:45:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kestrelvoice.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kestrelvoice-com/security/kestrelvoice-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Voice
- Platform
- ServiceBusinesses
- Integration
---
