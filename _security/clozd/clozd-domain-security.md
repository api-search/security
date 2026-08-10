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
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@clozd.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  caa_iodef: mailto:security@clozd.com
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clozd.com
  spf: true
hosts:
- cert_expires: Oct  1 23:41:30 2026 GMT
  host: www.clozd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: app.clozd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  http_status: 200
  https: true
  note: API host — serves /public-api/v1|v2|v3 and the Swagger UI at /public-api/docs/.
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: mcp.clozd.com
  hsts: false
  hsts_max_age_on_mcp_path: 31536000
  hsts_on_mcp_path: true
  http_status: 404
  https: true
  note: The host root returns 404 with no HSTS header; the MCP endpoint itself (POST /mcp) does return Strict-Transport-Security max-age=31536000; includeSubDomains along with nosniff, X-Frame-Options SAMEORIGIN, a restrictive CSP (default-src 'none'), COOP and CORP.
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: oauth.clozd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 404
  https: true
  note: Strongest HSTS posture of any Clozd host (2 years, preload).
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:00:49 2026 GMT
  host: help.clozd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 259200
  hsts_preload: false
  http_status: 302
  https: true
  note: Zendesk-hosted help center; blocks non-browser user agents with 403.
  tls_version: TLSv1.3
- host: trust.clozd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  http_status: 200
  https: true
  note: Vanta-hosted trust center.
kind: domain-security
layout: security
method: probed
name: Clozd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clozd, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clozd
provider_slug: clozd
slug: clozd-domain-security
source_filename: clozd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:41:30 2026 GMT\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: app.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: API host — serves /public-api/v1|v2|v3 and the Swagger UI at /public-api/docs/.\n- host: mcp.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  http_status: 404\n  hsts: false\n  hsts_on_mcp_path: true\n  hsts_max_age_on_mcp_path: 31536000\n  note: >-\n    The host root returns 404 with no HSTS header; the MCP endpoint itself (POST /mcp) does return\n    Strict-Transport-Security max-age=31536000;\
  \ includeSubDomains along with nosniff, X-Frame-Options\n    SAMEORIGIN, a restrictive CSP (default-src 'none'), COOP and CORP.\n- host: oauth.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  http_status: 404\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Strongest HSTS posture of any Clozd host (2 years, preload).\n- host: help.clozd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:00:49 2026 GMT\n  http_status: 302\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: Zendesk-hosted help center; blocks non-browser user agents with 403.\n- host: trust.clozd.com\n  https: true\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: Vanta-hosted trust center.\ndomains:\n- domain: clozd.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0\
  \ issuewild \"amazon.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@clozd.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  caa_iodef: mailto:security@clozd.com\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n- CAA is configured on the apex, including an iodef reporting address — above average for this catalog.\n- DMARC is published at p=quarantine rather than p=reject.\n- DNSSEC is not enabled on clozd.com.\n- HSTS is present on every host that serves content; mcp.clozd.com omits it on the host root.\nx-evidence:\n  fetched: '2026-08-04'\n  method_detail: >-\n    dig for CAA/SPF/DMARC/DNSSEC, openssl s_client for TLS version and certificate expiry, and curl -I for\n    HTTP status and Strict-Transport-Security per host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/security/clozd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- win-loss-analysis
- customer-feedback
- decision-intelligence
- sales-intelligence
- market-research
- competitive-intelligence
- voice-of-customer
- revenue-intelligence
- saas
- mcp
- agent-native
---
