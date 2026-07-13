---
api_specs:
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Repositories API
  slug: repositories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Runs and Checks API
  slug: runs-checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Analyzers API
  slug: analyzers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deepsource.com
  spf: false
hosts:
- cert_expires: Jul 21 16:02:22 2026 GMT
  host: deepsource.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 12:07:58 2026 GMT
  host: docs.deepsource.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:35:36 2026 GMT
  host: api.deepsource.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepsource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepSource, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: DeepSource
provider_slug: deepsource
slug: deepsource-domain-security
source_filename: deepsource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 16:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.deepsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.deepsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:35:36 2026 GMT\n  hsts: null\ndomains:\n- domain: deepsource.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/security/deepsource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Code Quality
- Static Analysis
- Code Review
- Security
- GraphQL
---
