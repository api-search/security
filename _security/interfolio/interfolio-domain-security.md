---
api_specs:
- filename: interfolio-activities-api-openapi.yml
  format: yaml
  label: Interfolio Activities API
  slug: interfolio-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activities-api-openapi.yml
- filename: interfolio-activity-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Activity Classifications API
  slug: interfolio-activity-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-classifications-api-openapi.yml
- filename: interfolio-activity-input-api-openapi.yml
  format: yaml
  label: Interfolio Activity Input API
  slug: interfolio-activity-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-input-api-openapi.yml
- filename: interfolio-courses-api-openapi.yml
  format: yaml
  label: Interfolio Courses API
  slug: interfolio-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-courses-api-openapi.yml
- filename: interfolio-download-attachments-api-openapi.yml
  format: yaml
  label: Interfolio Download Attachments API
  slug: interfolio-download-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-download-attachments-api-openapi.yml
- filename: interfolio-emails-api-openapi.yml
  format: yaml
  label: Interfolio Emails API
  slug: interfolio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-emails-api-openapi.yml
- filename: interfolio-evaluations-api-openapi.yml
  format: yaml
  label: Interfolio Evaluations API
  slug: interfolio-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-evaluations-api-openapi.yml
- filename: interfolio-faculty-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Faculty Classifications API
  slug: interfolio-faculty-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faculty-classifications-api-openapi.yml
- filename: interfolio-faq-api-openapi.yml
  format: yaml
  label: Interfolio FAQ API
  slug: interfolio-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faq-api-openapi.yml
- filename: interfolio-permissions-api-openapi.yml
  format: yaml
  label: Interfolio Permissions API
  slug: interfolio-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-permissions-api-openapi.yml
- filename: interfolio-sections-api-openapi.yml
  format: yaml
  label: Interfolio Sections API
  slug: interfolio-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sections-api-openapi.yml
- filename: interfolio-sso-api-openapi.yml
  format: yaml
  label: Interfolio SSO API
  slug: interfolio-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sso-api-openapi.yml
- filename: interfolio-terms-api-openapi.yml
  format: yaml
  label: Interfolio Terms API
  slug: interfolio-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-terms-api-openapi.yml
- filename: interfolio-units-api-openapi.yml
  format: yaml
  label: Interfolio Units API
  slug: interfolio-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-units-api-openapi.yml
- filename: interfolio-user-data-api-openapi.yml
  format: yaml
  label: Interfolio User Data API
  slug: interfolio-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-user-data-api-openapi.yml
- filename: interfolio-users-api-openapi.yml
  format: yaml
  label: Interfolio Users API
  slug: interfolio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-users-api-openapi.yml
- filename: interfolio-vitas-api-openapi.yml
  format: yaml
  label: Interfolio Vitas API
  slug: interfolio-vitas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-vitas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: interfolio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: faculty180.com
  spf: false
hosts:
- cert_expires: Nov 22 06:36:58 2026 GMT
  host: www.interfolio.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.faculty180.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  7 10:30:12 2027 GMT
  host: faculty180.interfolio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Interfolio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interfolio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Interfolio
provider_slug: interfolio
slug: interfolio-domain-security
source_filename: interfolio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interfolio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 06:36:58 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.faculty180.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: faculty180.interfolio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:30:12 2027 GMT\n  hsts: false\ndomains:\n- domain: interfolio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: faculty180.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/security/interfolio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Higher Education
- Faculty Information System
- Faculty Activity Reporting
- Review Promotion Tenure
- Academic
- Research
---
