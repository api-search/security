---
api_specs:
- filename: workera-audit-events-api-openapi.yml
  format: yaml
  label: Workera Audit Events API
  slug: workera-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-audit-events-api-openapi.yml
- filename: workera-benchmarks-api-openapi.yml
  format: yaml
  label: Workera Benchmarks API
  slug: workera-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-benchmarks-api-openapi.yml
- filename: workera-capability-api-openapi.yml
  format: yaml
  label: Workera Capability API
  slug: workera-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-capability-api-openapi.yml
- filename: workera-domains-api-openapi.yml
  format: yaml
  label: Workera Domains API
  slug: workera-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-domains-api-openapi.yml
- filename: workera-ping-api-openapi.yml
  format: yaml
  label: Workera Ping API
  slug: workera-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-ping-api-openapi.yml
- filename: workera-programs-api-openapi.yml
  format: yaml
  label: Workera Programs API
  slug: workera-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-programs-api-openapi.yml
- filename: workera-scores-api-openapi.yml
  format: yaml
  label: Workera Scores API
  slug: workera-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-scores-api-openapi.yml
- filename: workera-self-ratings-api-openapi.yml
  format: yaml
  label: Workera Self Ratings API
  slug: workera-self-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-self-ratings-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workera.ai
  spf: true
hosts:
- cert_expires: Nov  1 02:10:23 2026 GMT
  host: www.workera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: skills.workera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Workera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workera, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Workera
provider_slug: workera
slug: workera-domain-security
source_filename: workera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 02:10:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: skills.workera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workera.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/security/workera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Skills Intelligence
- Skills Assessment
- Human Resources
- Learning and Development
- Talent Management
- Workforce Analytics
- Artificial Intelligence
- Benchmarking
- Enterprise Software
- MCP
- Company
---
