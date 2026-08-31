---
api_specs:
- filename: phenom-applicants-api-openapi.yml
  format: yaml
  label: Phenom Applicants API
  slug: phenom-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-applicants-api-openapi.yml
- filename: phenom-applications-api-openapi.yml
  format: yaml
  label: Phenom Applications API
  slug: phenom-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-applications-api-openapi.yml
- filename: phenom-candidates-api-openapi.yml
  format: yaml
  label: Phenom Candidates API
  slug: phenom-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-candidates-api-openapi.yml
- filename: phenom-jobs-api-openapi.yml
  format: yaml
  label: Phenom Jobs API
  slug: phenom-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-jobs-api-openapi.yml
- filename: phenom-onboarding-api-openapi.yml
  format: yaml
  label: Phenom Onboarding API
  slug: phenom-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-onboarding-api-openapi.yml
- filename: phenom-parsers-api-openapi.yml
  format: yaml
  label: Phenom Parsers API
  slug: phenom-parsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-parsers-api-openapi.yml
- filename: phenom-prediction-api-openapi.yml
  format: yaml
  label: Phenom Prediction API
  slug: phenom-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-prediction-api-openapi.yml
- filename: phenom-tags-api-openapi.yml
  format: yaml
  label: Phenom Tags API
  slug: phenom-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-tags-api-openapi.yml
- filename: phenom-user-management-api-openapi.yml
  format: yaml
  label: Phenom User Management API
  slug: phenom-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: phenom.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: phenompro.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.phenom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: developer.phenom.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api-qa.phenompro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phenom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phenom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Phenom
provider_slug: phenom
slug: phenom-domain-security
source_filename: phenom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phenom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.phenom.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: api-qa.phenompro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phenom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: phenompro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/security/phenom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hr Tech
- Talent Experience
- Recruiting
- Applicant Tracking
- Candidate Experience
- Onboarding
- SCIM
- Resume Parsing
- Skills
- Artificial Intelligence
---
