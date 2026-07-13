---
api_specs:
- filename: candid-health-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: candid-health-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-openapi.yml
- filename: candid-health-openapi.yml
  format: yaml
  label: Candid Health Encounters API
  slug: candid-health-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-reporting@joincandidhealth.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: candidhealth.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caa-reporting@joincandidhealth.com"
  - 0 issue "pki.goog"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: joincandidhealth.com
  spf: true
hosts:
- cert_expires: Sep  1 15:33:55 2026 GMT
  host: candidhealth.com
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
name: Candid Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candid Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Candid Health
provider_slug: candid-health
slug: candid-health-domain-security
source_filename: candid-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: candidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:33:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joincandidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:54:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.joincandidhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:13:34 2026 GMT\n  hsts: null\ndomains:\n- domain: candidhealth.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:caa-reporting@joincandidhealth.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: joincandidhealth.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caa-reporting@joincandidhealth.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/security/candid-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Medical Billing
- Revenue Cycle Management
- Healthcare
- Claims
- Eligibility
- Prior Authorization
- Remittance
- Patient Collections
- Credentialing
- Insurance
---
