---
api_specs:
- filename: smartrecruiters-posting-openapi.yml
  format: yaml
  label: SmartRecruiters Posting API
  slug: posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-posting-openapi.yml
- filename: smartrecruiters-jobs-openapi.yml
  format: yaml
  label: SmartRecruiters Job API
  slug: job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-jobs-openapi.yml
- filename: smartrecruiters-candidates-openapi.yml
  format: yaml
  label: SmartRecruiters Candidate API
  slug: candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-candidates-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:caa@smartrecruiters.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: smartrecruiters.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.smartrecruiters.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:30:14 2026 GMT
  host: developers.smartrecruiters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.smartrecruiters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartrecruiters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartRecruiters, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SmartRecruiters
provider_slug: smartrecruiters
slug: smartrecruiters-domain-security
source_filename: smartrecruiters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartrecruiters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.smartrecruiters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:30:14 2026 GMT\n  hsts: null\n- host: api.smartrecruiters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartrecruiters.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:caa@smartrecruiters.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/security/smartrecruiters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Applicant Tracking
- HR Technology
---
