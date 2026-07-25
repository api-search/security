---
api_specs:
- filename: thriva-appointments-api-api-openapi.yml
  format: yaml
  label: Thriva Appointments API API
  slug: thriva-appointments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-appointments-api-api-openapi.yml
- filename: thriva-auth-api-api-openapi.yml
  format: yaml
  label: Thriva Auth API API
  slug: thriva-auth-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-auth-api-api-openapi.yml
- filename: thriva-biomarkers-api-api-openapi.yml
  format: yaml
  label: Thriva Biomarkers API API
  slug: thriva-biomarkers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-biomarkers-api-api-openapi.yml
- filename: thriva-bulk-orders-api-api-openapi.yml
  format: yaml
  label: Thriva Bulk Orders API API
  slug: thriva-bulk-orders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-bulk-orders-api-api-openapi.yml
- filename: thriva-escalations-api-api-openapi.yml
  format: yaml
  label: Thriva Escalations API API
  slug: thriva-escalations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-escalations-api-api-openapi.yml
- filename: thriva-orders-api-api-openapi.yml
  format: yaml
  label: Thriva Orders API API
  slug: thriva-orders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-orders-api-api-openapi.yml
- filename: thriva-result-attachments-api-api-openapi.yml
  format: yaml
  label: Thriva Result attachments API API
  slug: thriva-result-attachments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-result-attachments-api-api-openapi.yml
- filename: thriva-results-api-api-openapi.yml
  format: yaml
  label: Thriva Results API API
  slug: thriva-results-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-results-api-api-openapi.yml
- filename: thriva-tracking-api-api-openapi.yml
  format: yaml
  label: Thriva Tracking API API
  slug: thriva-tracking-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-tracking-api-api-openapi.yml
- filename: thriva-users-api-api-openapi.yml
  format: yaml
  label: Thriva Users API API
  slug: thriva-users-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-users-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thriva.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thriva.io
  spf: false
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: thriva.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.thriva.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api.euw2.sandbox.thriva.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thriva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thriva, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thriva
provider_slug: thriva
slug: thriva-domain-security
source_filename: thriva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thriva.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.thriva.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.euw2.sandbox.thriva.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thriva.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thriva.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/security/thriva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Diagnostics
- Blood Testing
- At-Home Testing
- Digital Health
- Lab Testing
- Webhooks
- United Kingdom
---
