---
api_specs:
- filename: geo-greeneris-openapi.yaml
  format: yaml
  label: geoscope
  slug: geoscope
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greeneris-io/openapi/geo-greeneris-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greeneris.io
  spf: true
hosts:
- cert_expires: Jan 11 14:31:39 2027 GMT
  host: greeneris.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GreenEris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GreenEris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GreenEris
provider_slug: greeneris-io
slug: greeneris-io-domain-security
source_filename: greeneris-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greeneris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:31:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: greeneris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/greeneris-io/security/greeneris-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Business
- GreenEris
---
