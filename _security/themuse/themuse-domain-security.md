---
api_specs:
- filename: themuse-companies-api-openapi.yml
  format: yaml
  label: The Muse Companies API
  slug: themuse-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themuse/refs/heads/main/openapi/themuse-companies-api-openapi.yml
- filename: themuse-jobs-api-openapi.yml
  format: yaml
  label: The Muse Jobs API
  slug: themuse-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themuse/refs/heads/main/openapi/themuse-jobs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: themuse.com
  spf: false
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.themuse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Themuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Muse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: The Muse
provider_slug: themuse
slug: themuse-domain-security
source_filename: themuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.themuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: themuse.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themuse/refs/heads/main/security/themuse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Openings
- Jobs
- Careers
- Recruiting
- Employment
- Company Profiles
- Job Search
- Hiring
- HR Tech
---
