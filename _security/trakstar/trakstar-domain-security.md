---
api_specs:
- filename: trakstar-auth-api-openapi.yml
  format: yaml
  label: Trakstar Auth API
  slug: trakstar-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-auth-api-openapi.yml
- filename: trakstar-candidate-messages-api-openapi.yml
  format: yaml
  label: Trakstar Candidate Messages API
  slug: trakstar-candidate-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-candidate-messages-api-openapi.yml
- filename: trakstar-candidates-api-openapi.yml
  format: yaml
  label: Trakstar Candidates API
  slug: trakstar-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-candidates-api-openapi.yml
- filename: trakstar-courses-api-openapi.yml
  format: yaml
  label: Trakstar Courses API
  slug: trakstar-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-courses-api-openapi.yml
- filename: trakstar-evaluations-api-openapi.yml
  format: yaml
  label: Trakstar Evaluations API
  slug: trakstar-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-evaluations-api-openapi.yml
- filename: trakstar-groups-api-openapi.yml
  format: yaml
  label: Trakstar Groups API
  slug: trakstar-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-groups-api-openapi.yml
- filename: trakstar-internal-notes-api-openapi.yml
  format: yaml
  label: Trakstar Internal Notes API
  slug: trakstar-internal-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-internal-notes-api-openapi.yml
- filename: trakstar-interviews-api-openapi.yml
  format: yaml
  label: Trakstar Interviews API
  slug: trakstar-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-interviews-api-openapi.yml
- filename: trakstar-openings-api-openapi.yml
  format: yaml
  label: Trakstar Openings API
  slug: trakstar-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-openings-api-openapi.yml
- filename: trakstar-reviews-api-openapi.yml
  format: yaml
  label: Trakstar Reviews API
  slug: trakstar-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-reviews-api-openapi.yml
- filename: trakstar-to-dos-api-openapi.yml
  format: yaml
  label: Trakstar To-Dos API
  slug: trakstar-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-to-dos-api-openapi.yml
- filename: trakstar-users-api-openapi.yml
  format: yaml
  label: Trakstar Users API
  slug: trakstar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trakstar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: recruiterbox.com
  spf: true
hosts:
- cert_expires: Sep 26 08:47:54 2026 GMT
  host: www.trakstar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 15:13:29 2026 GMT
  host: developers.recruiterbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: companyname.hire.trakstar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trakstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trakstar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trakstar
provider_slug: trakstar
slug: trakstar-domain-security
source_filename: trakstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trakstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:47:54 2026 GMT\n  hsts: false\n- host: developers.recruiterbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:13:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: companyname.hire.trakstar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trakstar.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: recruiterbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/security/trakstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- Performance Management
- Talent Management
- Applicant Tracking
- Learning Management
- 360 Feedback
- Goal Management
- Employee Development
- Performance Appraisal
---
