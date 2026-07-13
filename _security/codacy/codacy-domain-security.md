---
api_specs:
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Organizations API
  slug: organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Repositories API
  slug: repositories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Pull Requests API
  slug: pull-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Coverage API
  slug: coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Security API
  slug: security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
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
