---
api_specs:
- filename: zoho-recruit-candidates-api-openapi.yml
  format: yaml
  label: Zoho Recruit Candidates API
  slug: zoho-recruit-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-recruit/refs/heads/main/openapi/zoho-recruit-candidates-api-openapi.yml
- filename: zoho-recruit-job-openings-api-openapi.yml
  format: yaml
  label: Zoho Recruit Job Openings API
  slug: zoho-recruit-job-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-recruit/refs/heads/main/openapi/zoho-recruit-job-openings-api-openapi.yml
- filename: zoho-recruit-zoho-recruit-api-api-openapi.yml
  format: yaml
  label: Zoho Recruit Zoho Recruit API API
  slug: zoho-recruit-zoho-recruit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-recruit/refs/heads/main/openapi/zoho-recruit-zoho-recruit-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.zoho.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: recruit.zoho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoho Recruit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoho Recruit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoho Recruit
provider_slug: zoho-recruit
slug: zoho-recruit-domain-security
source_filename: zoho-recruit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: recruit.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoho.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-recruit/refs/heads/main/security/zoho-recruit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Applicant Tracking System
- ATS
- Recruiting
- Recruitment CRM
- HR
- Zoho
---
