---
api_specs:
- filename: pact_broker.json
  format: json
  label: Pact Broker API
  slug: pact-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/pact-foundation/pact_broker/master/lib/pact_broker/api/pact_broker.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cucumber.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pact.io
  spf: false
hosts:
- cert_expires: Sep 19 21:36:15 2026 GMT
  host: cucumber.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:33:41 2026 GMT
  host: docs.pact.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: stoplight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Test First Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test First, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Test First
provider_slug: test-first
slug: test-first-domain-security
source_filename: test-first-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cucumber.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:36:15 2026 GMT\n  hsts: false\n- host: docs.pact.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: false\ndomains:\n- domain: cucumber.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pact.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-first/refs/heads/main/security/test-first-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavior-Driven Development
- Best Practices
- Methodology
- Software Design
- Software Development
- Testing
---
