---
api_specs:
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Repos API
  slug: repos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Test Coverage API
  slug: test-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Snapshots API
  slug: snapshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Velocity API
  slug: velocity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: codeclimate.com
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: codeclimate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: developer.codeclimate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.codeclimate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codeclimate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code Climate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Code Climate
provider_slug: codeclimate
slug: codeclimate-domain-security
source_filename: codeclimate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codeclimate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.codeclimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.codeclimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codeclimate.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/security/codeclimate-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Code Quality
- Static Analysis
- Test Coverage
- Engineering Analytics
- DevOps
---
