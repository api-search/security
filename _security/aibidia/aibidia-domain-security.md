---
api_specs:
- filename: aibidia-aibidia-tp-ai-api-api-openapi.yml
  format: yaml
  label: Aibidia Aibidia TP AI API
  slug: aibidia-aibidia-tp-ai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-aibidia-tp-ai-api-api-openapi.yml
- filename: aibidia-authorize-api-openapi.yml
  format: yaml
  label: Aibidia Authorize API
  slug: aibidia-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-authorize-api-openapi.yml
- filename: aibidia-create-session-api-openapi.yml
  format: yaml
  label: Aibidia Create Session API
  slug: aibidia-create-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-create-session-api-openapi.yml
- filename: aibidia-datainjections-api-openapi.yml
  format: yaml
  label: Aibidia Data Injections API
  slug: aibidia-datainjections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-datainjections-api-openapi.yml
- filename: aibidia-extracttypes-api-openapi.yml
  format: yaml
  label: Aibidia Extract Types API
  slug: aibidia-extracttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-extracttypes-api-openapi.yml
- filename: aibidia-health-api-openapi.yml
  format: yaml
  label: Aibidia Health API
  slug: aibidia-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/openapi/aibidia-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aibidia.com
  spf: true
hosts:
- cert_expires: Nov 27 22:06:32 2026 GMT
  host: www.aibidia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 05:33:34 2026 GMT
  host: otpm-api.aibidia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 05:33:34 2026 GMT
  host: tpai-api.aibidia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aibidia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aibidia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aibidia
provider_slug: aibidia
slug: aibidia-domain-security
source_filename: aibidia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aibidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 22:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: otpm-api.aibidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 05:33:34 2026 GMT\n  hsts: null\n- host: tpai-api.aibidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 05:33:34 2026 GMT\n  hsts: null\ndomains:\n- domain: aibidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aibidia/refs/heads/main/security/aibidia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Transfer Pricing
- Tax Technology
- Tax Compliance
- Regulatory Reporting
- Country-by-Country Reporting
- Financial Data
- Enterprise Software
- Data Ingestion
- Finland
---
