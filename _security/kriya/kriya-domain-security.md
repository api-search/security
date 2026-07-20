---
api_specs:
- filename: kriya-payments-openapi.yaml
  format: yaml
  label: Kriya Payments API
  slug: kriya-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/openapi/kriya-payments-openapi.yaml
- filename: kriya-onboarding-openapi.yaml
  format: yaml
  label: Kriya Onboarding API
  slug: kriya-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/openapi/kriya-onboarding-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kriya.co
  spf: true
hosts:
- cert_expires: Sep 11 12:30:14 2026 GMT
  host: www.kriya.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 09:31:11 2026 GMT
  host: docs.kriya.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:09:27 2026 GMT
  host: api.kriya.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kriya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kriya, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kriya
provider_slug: kriya
slug: kriya-domain-security
source_filename: kriya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kriya.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kriya.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kriya.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:09:27 2026 GMT\n  hsts: null\ndomains:\n- domain: kriya.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/security/kriya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Buy Now Pay Later
- B2B Payments
- Invoice Finance
- Lending
- Working Capital
- Onboarding
- KYC
- United Kingdom
---
