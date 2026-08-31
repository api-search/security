---
api_specs:
- filename: vim-access-token-retrieval-api-openapi.yml
  format: yaml
  label: Vim Access Token Retrieval API
  slug: vim-access-token-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-access-token-retrieval-api-openapi.yml
- filename: vim-applications-api-openapi.yml
  format: yaml
  label: Vim Applications API
  slug: vim-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-applications-api-openapi.yml
- filename: vim-appointments-api-openapi.yml
  format: yaml
  label: Vim Appointments API
  slug: vim-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-appointments-api-openapi.yml
- filename: vim-authentication-api-openapi.yml
  format: yaml
  label: Vim Authentication API
  slug: vim-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-authentication-api-openapi.yml
- filename: vim-chart-retrieval-api-openapi.yml
  format: yaml
  label: Vim Chart Retrieval API
  slug: vim-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-chart-retrieval-api-openapi.yml
- filename: vim-get-patient-care-insights-api-openapi.yml
  format: yaml
  label: Vim Get Patient Care Insights API
  slug: vim-get-patient-care-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-get-patient-care-insights-api-openapi.yml
- filename: vim-invitations-api-openapi.yml
  format: yaml
  label: Vim Invitations API
  slug: vim-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-invitations-api-openapi.yml
- filename: vim-patient-care-insights-feedback-api-openapi.yml
  format: yaml
  label: Vim Patient Care Insights Feedback API
  slug: vim-patient-care-insights-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-patient-care-insights-feedback-api-openapi.yml
- filename: vim-patient-identification-api-openapi.yml
  format: yaml
  label: Vim Patient Identification API
  slug: vim-patient-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-patient-identification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getvim.com
  spf: true
hosts:
- cert_expires: Nov 10 03:45:42 2026 GMT
  host: getvim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 20:43:02 2026 GMT
  host: docs.getvim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:13:22 2026 GMT
  host: api.getvim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vim, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vim
provider_slug: vim
slug: vim-domain-security
source_filename: vim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 03:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 20:43:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:13:22 2026 GMT\n  hsts: null\ndomains:\n- domain: getvim.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/security/vim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Clinical AI
- EHR Integration
- Point of Care
- Interoperability
- Value-Based Care
- Care Gaps
- Authentication
---
