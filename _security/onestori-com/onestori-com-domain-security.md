---
api_specs:
- filename: onestori-com-ai-api-openapi.yml
  format: yaml
  label: Stori AI API
  slug: onestori-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-ai-api-openapi.yml
- filename: onestori-com-billing-api-openapi.yml
  format: yaml
  label: Stori Billing API
  slug: onestori-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-billing-api-openapi.yml
- filename: onestori-com-email-api-openapi.yml
  format: yaml
  label: Stori Email API
  slug: onestori-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-email-api-openapi.yml
- filename: onestori-com-jobs-api-openapi.yml
  format: yaml
  label: Stori Jobs API
  slug: onestori-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-jobs-api-openapi.yml
- filename: onestori-com-partner-api-v1-api-openapi.yml
  format: yaml
  label: Stori Partner API v1 API
  slug: onestori-com-partner-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-partner-api-v1-api-openapi.yml
- filename: onestori-com-profile-api-openapi.yml
  format: yaml
  label: Stori Profile API
  slug: onestori-com-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-profile-api-openapi.yml
- filename: onestori-com-recruiter-api-openapi.yml
  format: yaml
  label: Stori Recruiter API
  slug: onestori-com-recruiter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-recruiter-api-openapi.yml
- filename: onestori-com-traits-api-openapi.yml
  format: yaml
  label: Stori Traits API
  slug: onestori-com-traits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-traits-api-openapi.yml
- filename: onestori-com-video-api-openapi.yml
  format: yaml
  label: Stori Video API
  slug: onestori-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-video-api-openapi.yml
- filename: onestori-com-webhooks-api-openapi.yml
  format: yaml
  label: Stori Webhooks API
  slug: onestori-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onestori.com
  spf: true
hosts:
- cert_expires: Jan 20 18:49:05 2027 GMT
  host: onestori.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stori
provider_slug: onestori-com
slug: onestori-com-domain-security
source_filename: onestori-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onestori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:49:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onestori.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/onestori-com/security/onestori-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hiring
- Artificial Intelligence
- Candidate Intelligence
- Recruiting
---
