---
api_specs:
- filename: generate-a-client-from-openapi-definition
  format: yaml
  label: Moody's KYC API
  slug: moodys
  spec_type: OpenAPI
  url: 'https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/

    https://www.kompany.com/kycapi/docs/resources/resources/customer-facing-documents/generate-a-client-from-openapi-definition'
- filename: moodys-data-buffet-api-openapi.yml
  format: yaml
  label: Moody's Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-data-buffet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moodysanalytics.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.kompany.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: hub.moodysanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:57:38 2026 GMT
  host: developer.rms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moodys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moody''s, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moody's
provider_slug: moodys
slug: moodys-domain-security
source_filename: moodys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\n- host: hub.moodysanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:57:38 2026 GMT\n  hsts: null\ndomains:\n- domain: kompany.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moodysanalytics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/security/moodys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
---
