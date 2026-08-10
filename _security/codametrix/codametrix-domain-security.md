---
api_specs:
- filename: codametrix-components-api-openapi.yml
  format: yaml
  label: CodaMetrix Components API
  slug: codametrix-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-components-api-openapi.yml
- filename: codametrix-incidents-api-openapi.yml
  format: yaml
  label: CodaMetrix Incidents API
  slug: codametrix-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-incidents-api-openapi.yml
- filename: codametrix-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: CodaMetrix Scheduled Maintenances API
  slug: codametrix-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-scheduled-maintenances-api-openapi.yml
- filename: codametrix-status-api-openapi.yml
  format: yaml
  label: CodaMetrix Status API
  slug: codametrix-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-status-api-openapi.yml
- filename: codametrix-summary-api-openapi.yml
  format: yaml
  label: CodaMetrix Summary API
  slug: codametrix-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-summary-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codametrix.com
  spf: true
hosts:
- cert_expires: Sep 10 15:01:35 2026 GMT
  host: www.codametrix.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  platform: Webflow behind Cloudflare
  tls_version: TLSv1.3
- api_host: true
  cert_expires: Sep 17 05:22:09 2026 GMT
  host: status.codametrix.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 259200
  https: true
  platform: Atlassian Statuspage behind CloudFront (AtlassianEdge)
  tls_version: TLSv1.3
- host: trust.codametrix.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  platform: Vanta Trust Center
kind: domain-security
layout: security
method: probed
name: Codametrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodaMetrix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodaMetrix
provider_slug: codametrix
slug: codametrix-domain-security
source_filename: codametrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI servers hosts\nnote: >-\n  HSTS values were read directly from the strict-transport-security response header on each host\n  (curl -D -). The mechanical probe returned null for HSTS on this run; the header is present on all three\n  hosts and the observed values are recorded here.\nhosts:\n- host: www.codametrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  platform: Webflow behind Cloudflare\n- host: status.codametrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:22:09 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: false\n  platform: Atlassian Statuspage behind CloudFront (AtlassianEdge)\n  api_host: true\n- host: trust.codametrix.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains:\
  \ true\n  platform: Vanta Trust Center\ndomains:\n- domain: codametrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\napi_response_security_headers:\n  host: status.codametrix.com\n  x_content_type_options: nosniff\n  x_xss_protection: 1; mode=block\n  x_download_options: noopen\n  x_permitted_cross_domain_policies: none\n  referrer_policy: strict-origin-when-cross-origin\n  access_control_allow_origin: '*'\n  note: The wide-open CORS policy is intentional for a public status API and is not a finding.\ngaps:\n- No DNSSEC on codametrix.com.\n- No CAA records, so any public CA may issue for the domain.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://www.codametrix.com/', http_status: 200, header: 'strict-transport-security: max-age=31536000'}\n  - {url: 'https://status.codametrix.com/', http_status: 200, header: 'strict-transport-security: max-age=259200'}\n  - {url: 'https://trust.codametrix.com/', http_status: 200, header: 'strict-transport-security:\
  \ max-age=31536000; includeSubDomains'}\n  - {url: 'https://status.codametrix.com/api/v2/summary.json', http_status: 200, note: API response security headers read here}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/security/codametrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- healthcare
- health-systems
- medical-coding
- autonomous-coding
- revenue-cycle-management
- clinical-documentation
- healthcare-ai
- machine-learning
- natural-language-processing
- ehr-integration
- status
---
