---
api_specs:
- filename: moodys-analytics-developer-openapi.yml
  format: yaml
  label: Moody's Analytics Developer Platform
  slug: developer-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/openapi/moodys-analytics-developer-openapi.yml
- filename: moodys-data-buffet-api-openapi.yml
  format: yaml
  label: Moody's Analytics Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/openapi/moodys-data-buffet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moodys.com
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: www.moodys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: ratings.moodys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.moodys.com
  https: false
kind: domain-security
layout: security
method: probed
name: Moodys Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moody''s Corporation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moody's Corporation
provider_slug: moodys-corporation
slug: moodys-corporation-domain-security
source_filename: moodys-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moodys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ratings.moodys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.moodys.com\n  https: false\ndomains:\n- domain: moodys.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/security/moodys-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Catastrophe Risk
- Climate Risk
- Compliance
- Credit Ratings
- Economic Data
- ESG
- Financial Data
- KYC
- Risk
- Fortune 1000
---
