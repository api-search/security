---
api_specs:
- filename: 42crunch-scand-manager.yaml
  format: yaml
  label: 42Crunch API Conformance Scan Jobs Manager
  slug: 42crunch-scand-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/openapi/42crunch-scand-manager.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 42crunch.com
  spf: true
hosts:
- cert_expires: Oct  6 23:38:08 2026 GMT
  host: 42crunch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:07:30 2026 GMT
  host: docs.42crunch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 42Crunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 42Crunch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 42Crunch
provider_slug: 42crunch
slug: 42crunch-domain-security
source_filename: 42crunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 42crunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.42crunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:07:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 42crunch.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/security/42crunch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
---
