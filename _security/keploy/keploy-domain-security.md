---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keploy.io
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: keploy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 02:28:07 2026 GMT
  host: api.keploy.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keploy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keploy
provider_slug: keploy
slug: keploy-domain-security
source_filename: keploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keploy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.keploy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:28:07 2026 GMT\n  hsts: null\ndomains:\n- domain: keploy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/security/keploy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing & QA
- API Testing
- Integration/Regression Testing
- Unit Test Generation
- Contract Testing
- CI/CD
- Developer Tools
- AI / Agent Tooling
- eBPF / Observability
- Test Data & Mocking
---
