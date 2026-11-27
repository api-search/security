---
api_specs:
- filename: hillsignal-com-openapi-generated.yml
  format: yaml
  label: HillSignal API
  slug: hillsignal-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hillsignal-com/openapi/_ae-authored/hillsignal-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hillsignal.com
  spf: true
hosts:
- cert_expires: Dec 15 19:22:17 2026 GMT
  host: hillsignal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HillSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HillSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HillSignal
provider_slug: hillsignal-com
slug: hillsignal-com-domain-security
source_filename: hillsignal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hillsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:22:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hillsignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hillsignal-com/security/hillsignal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HillSignal
- Data Intelligence
- Government
- Finance
---
