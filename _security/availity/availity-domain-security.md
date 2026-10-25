---
api_specs:
- filename: availity-auth-attachments-api-openapi.yml
  format: yaml
  label: availity Auth Attachments API
  slug: availity-auth-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-auth-attachments-api-openapi.yml
- filename: availity-claim-attachments-api-openapi.yml
  format: yaml
  label: availity Claim Attachments API
  slug: availity-claim-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-attachments-api-openapi.yml
- filename: availity-claim-status-api-openapi.yml
  format: yaml
  label: availity Claim Status API
  slug: availity-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-status-api-openapi.yml
- filename: availity-eligibility-api-openapi.yml
  format: yaml
  label: availity Eligibility API
  slug: availity-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-eligibility-api-openapi.yml
- filename: availity-enhanced-claim-status-api-openapi.yml
  format: yaml
  label: availity Enhanced Claim Status API
  slug: availity-enhanced-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-enhanced-claim-status-api-openapi.yml
- filename: availity-is-auth-required-api-openapi.yml
  format: yaml
  label: availity Is Auth Required API
  slug: availity-is-auth-required-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-is-auth-required-api-openapi.yml
- filename: availity-service-reviews-api-openapi.yml
  format: yaml
  label: availity Service Reviews API
  slug: availity-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-service-reviews-api-openapi.yml
- filename: availity-availity-payer-list-api-openapi.yml
  format: yaml
  label: Availity Availity Payer List API
  slug: availity-availity-payer-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-availity-payer-list-api-openapi.yml
- filename: availity-claim-statuses-api-openapi.yml
  format: yaml
  label: Availity Claim Statuses API
  slug: availity-claim-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-statuses-api-openapi.yml
- filename: availity-configurations-api-openapi.yml
  format: yaml
  label: Availity Configurations API
  slug: availity-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-configurations-api-openapi.yml
- filename: availity-coverages-api-openapi.yml
  format: yaml
  label: Availity Coverages API
  slug: availity-coverages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-coverages-api-openapi.yml
- filename: availity-dental-claims-api-openapi.yml
  format: yaml
  label: Availity Dental Claims API
  slug: availity-dental-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-dental-claims-api-openapi.yml
- filename: availity-dfs-api-openapi.yml
  format: yaml
  label: Availity Dfs API
  slug: availity-dfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-dfs-api-openapi.yml
- filename: availity-institutional-claims-api-openapi.yml
  format: yaml
  label: Availity Institutional Claims API
  slug: availity-institutional-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-institutional-claims-api-openapi.yml
- filename: availity-patient-cost-estimator-2-0-0-professional-api-openapi.yml
  format: yaml
  label: Availity Patient Cost Estimator 2.0.0 Professional API
  slug: availity-patient-cost-estimator-2-0-0-professional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-patient-cost-estimator-2-0-0-professional-api-openapi.yml
- filename: availity-professional-claims-api-openapi.yml
  format: yaml
  label: Availity Professional Claims API
  slug: availity-professional-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-professional-claims-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: availity.com
  spf: true
hosts:
- cert_expires: Dec  5 19:51:32 2026 GMT
  host: www.availity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: developer.availity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.availity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Availity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Availity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Availity
provider_slug: availity
slug: availity-domain-security
source_filename: availity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.availity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 19:51:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.availity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: false\n- host: api.availity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: availity.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/security/availity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Clearinghouse
- HIPAA
- X12 EDI
- Eligibility
- Claims
- Prior Authorization
- Revenue Cycle Management
- Payers
- Price Transparency
- Health Insurance
---
