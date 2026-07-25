---
api_specs:
- filename: hyperscience-audit-logs-api-openapi.yml
  format: yaml
  label: Hyperscience Audit Logs API
  slug: hyperscience-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-audit-logs-api-openapi.yml
- filename: hyperscience-cases-api-openapi.yml
  format: yaml
  label: Hyperscience Cases API
  slug: hyperscience-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-cases-api-openapi.yml
- filename: hyperscience-documents-api-openapi.yml
  format: yaml
  label: Hyperscience Documents API
  slug: hyperscience-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-documents-api-openapi.yml
- filename: hyperscience-flow-runs-api-openapi.yml
  format: yaml
  label: Hyperscience Flow Runs API
  slug: hyperscience-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flow-runs-api-openapi.yml
- filename: hyperscience-flows-api-openapi.yml
  format: yaml
  label: Hyperscience Flows API
  slug: hyperscience-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flows-api-openapi.yml
- filename: hyperscience-layouts-api-openapi.yml
  format: yaml
  label: Hyperscience Layouts API
  slug: hyperscience-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-layouts-api-openapi.yml
- filename: hyperscience-pages-api-openapi.yml
  format: yaml
  label: Hyperscience Pages API
  slug: hyperscience-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-pages-api-openapi.yml
- filename: hyperscience-submissions-api-openapi.yml
  format: yaml
  label: Hyperscience Submissions API
  slug: hyperscience-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-submissions-api-openapi.yml
- filename: hyperscience-version-api-openapi.yml
  format: yaml
  label: Hyperscience Version API
  slug: hyperscience-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperscience.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperscience.net
  spf: true
hosts:
- cert_expires: Aug 24 09:38:30 2026 GMT
  host: www.hyperscience.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: <tenant>.hyperscience.net
  https: false
kind: domain-security
layout: security
method: probed
name: Hyperscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperscience, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperscience
provider_slug: hyperscience
slug: hyperscience-domain-security
source_filename: hyperscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperscience.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: <tenant>.hyperscience.net\n  https: false\ndomains:\n- domain: hyperscience.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hyperscience.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/security/hyperscience-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document AI
- IDP
- Enterprise
- Automation
- GenAI
- FedRAMP
---
