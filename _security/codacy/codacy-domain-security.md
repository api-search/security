---
api_specs:
- filename: codacy-account-api-openapi.yml
  format: yaml
  label: Codacy Account API
  slug: codacy-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-account-api-openapi.yml
- filename: codacy-coverage-api-openapi.yml
  format: yaml
  label: Codacy Coverage API
  slug: codacy-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-coverage-api-openapi.yml
- filename: codacy-issues-api-openapi.yml
  format: yaml
  label: Codacy Issues API
  slug: codacy-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-issues-api-openapi.yml
- filename: codacy-organizations-api-openapi.yml
  format: yaml
  label: Codacy Organizations API
  slug: codacy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-organizations-api-openapi.yml
- filename: codacy-pull-requests-api-openapi.yml
  format: yaml
  label: Codacy Pull Requests API
  slug: codacy-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-pull-requests-api-openapi.yml
- filename: codacy-quality-settings-api-openapi.yml
  format: yaml
  label: Codacy Quality Settings API
  slug: codacy-quality-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-quality-settings-api-openapi.yml
- filename: codacy-repositories-api-openapi.yml
  format: yaml
  label: Codacy Repositories API
  slug: codacy-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-repositories-api-openapi.yml
- filename: codacy-security-api-openapi.yml
  format: yaml
  label: Codacy Security API
  slug: codacy-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-security-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codacy.com
  spf: true
hosts:
- cert_expires: Aug 23 13:10:32 2026 GMT
  host: www.codacy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 00:13:18 2026 GMT
  host: docs.codacy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.codacy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codacy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Codacy
provider_slug: codacy
slug: codacy-domain-security
source_filename: codacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:10:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.codacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:13:18 2026 GMT\n  hsts: false\n- host: api.codacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codacy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/security/codacy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Quality
- Static Analysis
- Security
- Code Coverage
- DevOps
---
