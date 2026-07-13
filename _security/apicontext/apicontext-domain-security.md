---
api_specs:
- filename: apicontext-platform-openapi.yaml
  format: yaml
  label: APIContext Synthetic API Testing
  slug: synthetic-api-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-platform-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apicontext.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: apimetrics.io
  spf: true
hosts:
- cert_expires: Aug 26 01:03:06 2026 GMT
  host: apicontext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 09:48:31 2026 GMT
  host: client.apimetrics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apicontext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIContext, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APIContext
provider_slug: apicontext
slug: apicontext-domain-security
source_filename: apicontext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apicontext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:03:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: client.apimetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:48:31 2026 GMT\n  hsts: false\ndomains:\n- domain: apicontext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apimetrics.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/security/apicontext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Directory
- API Monitoring
- Conformance
- Performance
- Platform
- SLO
- Synthetic Testing
- Testing
---
