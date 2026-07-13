---
api_specs:
- filename: k6-openapi.yml
  format: yaml
  label: K6
  slug: k6
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/k6/refs/heads/main/openapi/k6-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: k6.io
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: k6.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.k6.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: K6 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for K6, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: K6
provider_slug: k6
slug: k6-domain-security
source_filename: k6-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: k6.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.k6.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: k6.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k6/refs/heads/main/security/k6-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Load Testing
- Testing
---
