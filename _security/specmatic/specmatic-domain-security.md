---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: specmatic.io
  spf: true
hosts:
- cert_expires: Oct  1 23:03:51 2026 GMT
  host: specmatic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: app.specmatic.io
  https: false
kind: domain-security
layout: security
method: probed
name: Specmatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Specmatic, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Specmatic
provider_slug: specmatic
slug: specmatic-domain-security
source_filename: specmatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: specmatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:03:51 2026 GMT\n  hsts: false\n- host: app.specmatic.io\n  https: false\ndomains:\n- domain: specmatic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specmatic/refs/heads/main/security/specmatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Contract Testing
- API Governance
- API Mocking
- Backward Compatibility
- Contract-Driven Development
- Service Virtualization
---
