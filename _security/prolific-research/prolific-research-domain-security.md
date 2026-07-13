---
api_specs:
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Studies API
  slug: prolific-research-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Submissions API
  slug: prolific-research-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Participant Groups API
  slug: prolific-research-participant-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Projects API
  slug: prolific-research-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Workspaces API
  slug: prolific-research-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Messages API
  slug: prolific-research-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Hooks (Webhooks) API
  slug: prolific-research-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Requirements & Filters API
  slug: prolific-research-requirements-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Bonuses API
  slug: prolific-research-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Users API
  slug: prolific-research-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: prolific.com
  spf: true
hosts:
- cert_expires: Aug 29 12:36:41 2026 GMT
  host: www.prolific.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 21:01:54 2026 GMT
  host: docs.prolific.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:47:44 2026 GMT
  host: api.prolific.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prolific Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prolific, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Prolific
provider_slug: prolific-research
slug: prolific-research-domain-security
source_filename: prolific-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prolific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:36:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.prolific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prolific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:47:44 2026 GMT\n  hsts: null\ndomains:\n- domain: prolific.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/security/prolific-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Research
- Participant Recruitment
- Surveys
- Human Data
- Crowdsourcing
- Data Annotation
- AI Training
---
