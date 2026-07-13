---
api_specs:
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Job Sync API
  slug: job-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Employer API
  slug: employer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: indeed.com
  spf: true
hosts:
- cert_expires: Aug 30 03:04:10 2026 GMT
  host: developer.indeed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.indeed.com
  https: false
- cert_expires: Sep 15 01:33:20 2026 GMT
  host: www.indeed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indeed, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Indeed
provider_slug: indeed
slug: indeed-domain-security
source_filename: indeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.indeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:04:10 2026 GMT\n  hsts: null\n- host: api.indeed.com\n  https: false\n- host: www.indeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:33:20 2026 GMT\n  hsts: null\ndomains:\n- domain: indeed.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/security/indeed-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
---
