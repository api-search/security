---
api_specs:
- filename: signalhouse-io-openapi-generated.yml
  format: yaml
  label: Signal House API
  slug: signalhouse-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalhouse-io/openapi/_ae-authored/signalhouse-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signalhouse.io
  spf: true
hosts:
- cert_expires: Feb  7 00:45:58 2027 GMT
  host: signalhouse.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signal House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signal House, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Signal House
provider_slug: signalhouse-io
slug: signalhouse-io-domain-security
source_filename: signalhouse-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signalhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 00:45:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signalhouse.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signalhouse-io/security/signalhouse-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- MMS
- Voice
- CPaaS
- 10DLC
- Messaging APIs
- Voice APIs
- A2P
---
