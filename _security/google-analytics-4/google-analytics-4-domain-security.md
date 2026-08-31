---
api_specs:
- filename: google-analytics-4-accounts-api-openapi.yml
  format: yaml
  label: Google Analytics 4 Accounts API
  slug: google-analytics-4-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-accounts-api-openapi.yml
- filename: google-analytics-4-accountsummaries-api-openapi.yml
  format: yaml
  label: Google Analytics 4 Account Summaries API
  slug: google-analytics-4-accountsummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-accountsummaries-api-openapi.yml
- filename: google-analytics-4-properties-api-openapi.yml
  format: yaml
  label: Google Analytics 4 Properties API
  slug: google-analytics-4-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-properties-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google-analytics.com
  spf: true
hosts:
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: www.google-analytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: analyticsdata.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Analytics 4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Analytics 4, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Analytics 4
provider_slug: google-analytics-4
slug: google-analytics-4-domain-security
source_filename: google-analytics-4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.google-analytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: false\n- host: analyticsdata.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google-analytics.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/security/google-analytics-4-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data Collection
- Marketing
- Measurements
- Mobile Analytics
- Reporting
- Web Analytics
- Attribution
- Audiences
- Event Tracking
---
