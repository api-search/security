---
api_specs:
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Encounters & Claims API
  slug: encounters-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Charge Capture API
  slug: charge-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Payers & Fee Schedules API
  slug: payers-fee-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Remits & ERAs API
  slug: remits-eras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Webhooks & Events API
  slug: webhooks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
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
