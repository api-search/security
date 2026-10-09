---
api_specs:
- filename: kognitos-analytics-api-openapi.yml
  format: yaml
  label: Kognitos Analytics API
  slug: kognitos-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-analytics-api-openapi.yml
- filename: kognitos-automations-api-openapi.yml
  format: yaml
  label: Kognitos Automations API
  slug: kognitos-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-automations-api-openapi.yml
- filename: kognitos-books-api-openapi.yml
  format: yaml
  label: Kognitos Books API
  slug: kognitos-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-books-api-openapi.yml
- filename: kognitos-exceptions-api-openapi.yml
  format: yaml
  label: Kognitos Exceptions API
  slug: kognitos-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-exceptions-api-openapi.yml
- filename: kognitos-files-api-openapi.yml
  format: yaml
  label: Kognitos Files API
  slug: kognitos-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-files-api-openapi.yml
- filename: kognitos-organizations-api-openapi.yml
  format: yaml
  label: Kognitos Organizations API
  slug: kognitos-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-organizations-api-openapi.yml
- filename: kognitos-runs-api-openapi.yml
  format: yaml
  label: Kognitos Runs API
  slug: kognitos-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-runs-api-openapi.yml
- filename: kognitos-workspaces-api-openapi.yml
  format: yaml
  label: Kognitos Workspaces API
  slug: kognitos-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: kognitos.com
  spf: true
hosts:
- cert_expires: Nov 25 16:45:51 2026 GMT
  host: www.kognitos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 12:05:03 2026 GMT
  host: docs.kognitos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 21 23:59:59 2027 GMT
  host: app.us-1.kognitos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Kognitos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kognitos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Kognitos
provider_slug: kognitos
slug: kognitos-domain-security
source_filename: kognitos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kognitos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 16:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kognitos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:05:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.us-1.kognitos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kognitos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/security/kognitos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agentic AI
- Automation
- Workflow Automation
- Finance Automation
- Accounts Payable
- Neurosymbolic AI
- Enterprise
---
