---
api_specs:
- filename: clozd-programs-api-openapi.yml
  format: yaml
  label: Clozd /programs API
  slug: clozd-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-api-openapi.yml
- filename: clozd-programs-program-id-competitors-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/competitors API
  slug: clozd-programs-program-id-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-competitors-api-openapi.yml
- filename: clozd-programs-program-id-deals-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals API
  slug: clozd-programs-program-id-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-api-openapi.yml
- filename: clozd-programs-program-id-deals-deal-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/:deal ID API
  slug: clozd-programs-program-id-deals-deal-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-deal-id-api-openapi.yml
- filename: clozd-programs-program-id-deals-import-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/import API
  slug: clozd-programs-program-id-deals-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-import-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints API
  slug: clozd-programs-program-id-touchpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints/:touchpoint ID API
  slug: clozd-programs-program-id-touchpoints-touchpoint-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@clozd.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clozd.com
  spf: true
hosts:
- cert_expires: Oct  1 23:41:30 2026 GMT
  host: www.clozd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:00:49 2026 GMT
  host: help.clozd.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: mcp.clozd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clozd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clozd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clozd
provider_slug: clozd
slug: clozd-domain-security
source_filename: clozd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:41:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: mcp.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: clozd.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@clozd.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/security/clozd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- win-loss-analysis
- customer-feedback
- decision-intelligence
- sales-intelligence
- market-research
- Competitive Intelligence
- voice-of-customer
- revenue-intelligence
- saas
- MCP
- agent-native
---
