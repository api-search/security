---
api_specs:
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applicants API
  slug: applicants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Job Stages API
  slug: job-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Comments and Files API
  slug: comments-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinpointhq.com
  spf: true
hosts:
- cert_expires: Sep 30 13:45:35 2026 GMT
  host: www.pinpointhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:23:34 2026 GMT
  host: developers.pinpointhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinpoint, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinpoint
provider_slug: pinpoint
slug: pinpoint-domain-security
source_filename: pinpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinpointhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:45:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.pinpointhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pinpointhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/security/pinpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATS
- Recruitment
- Hiring
- HR Tech
- JSON:API
---
