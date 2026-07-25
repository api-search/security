---
api_specs:
- filename: candidhealth-auth-api-openapi.yml
  format: yaml
  label: Candid Health Auth API
  slug: candidhealth-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-auth-api-openapi.yml
- filename: candidhealth-charge-capture-api-openapi.yml
  format: yaml
  label: Candid Health Charge Capture API
  slug: candidhealth-charge-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-charge-capture-api-openapi.yml
- filename: candidhealth-eligibility-api-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: candidhealth-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-eligibility-api-openapi.yml
- filename: candidhealth-encounters-api-openapi.yml
  format: yaml
  label: Candid Health Encounters API
  slug: candidhealth-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-encounters-api-openapi.yml
- filename: candidhealth-events-api-openapi.yml
  format: yaml
  label: Candid Health Events API
  slug: candidhealth-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-events-api-openapi.yml
- filename: candidhealth-fee-schedules-api-openapi.yml
  format: yaml
  label: Candid Health Fee Schedules API
  slug: candidhealth-fee-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-fee-schedules-api-openapi.yml
- filename: candidhealth-insurance-adjudications-api-openapi.yml
  format: yaml
  label: Candid Health Insurance Adjudications API
  slug: candidhealth-insurance-adjudications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-insurance-adjudications-api-openapi.yml
- filename: candidhealth-payers-api-openapi.yml
  format: yaml
  label: Candid Health Payers API
  slug: candidhealth-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-payers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-reporting@joincandidhealth.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: joincandidhealth.com
  spf: true
hosts:
- cert_expires: Sep 28 21:18:06 2026 GMT
  host: www.joincandidhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:54:12 2026 GMT
  host: docs.joincandidhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 18:13:34 2026 GMT
  host: api.joincandidhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Candidhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candid Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Candid Health
provider_slug: candidhealth
slug: candidhealth-domain-security
source_filename: candidhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joincandidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:18:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joincandidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:54:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.joincandidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:13:34 2026 GMT\n  hsts: null\ndomains:\n- domain: joincandidhealth.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:caa-reporting@joincandidhealth.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/security/candidhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Medical Billing
- Revenue Cycle
- Claims
- Eligibility
---
