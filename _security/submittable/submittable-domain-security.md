---
api_specs:
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Submissions API
  slug: submittable-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Entries API
  slug: submittable-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Projects and Forms API
  slug: submittable-projects-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Users (Submitters) API
  slug: submittable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Teams and Reviews API
  slug: submittable-teams-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Labels API
  slug: submittable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Funds and Payments API
  slug: submittable-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: submittable.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: submittable.help
  spf: false
hosts:
- cert_expires: Sep 21 20:02:28 2026 GMT
  host: www.submittable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: submittable-api.submittable.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: submittable.help
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Submittable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Submittable, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Submittable
provider_slug: submittable
slug: submittable-domain-security
source_filename: submittable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.submittable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: submittable-api.submittable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: submittable.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: submittable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: submittable.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/security/submittable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Submission Management
- Grants Management
- Applications
- Forms
- Nonprofit
- Corporate Social Responsibility
- Workflow
---
