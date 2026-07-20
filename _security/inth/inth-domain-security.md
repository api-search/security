---
api_specs:
- filename: inth-c15t-consent-api.yml
  format: yaml
  label: c15t Consent Backend API
  slug: c15t-consent-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inth/refs/heads/main/openapi/inth-c15t-consent-api.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: c15t.com
  spf: false
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: c15t.dev
  spf: false
hosts:
- cert_expires: Sep 22 02:33:23 2026 GMT
  host: c15t.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 20:57:33 2026 GMT
  host: your-instance.c15t.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inth, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Inth
provider_slug: inth
slug: inth-domain-security
source_filename: inth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: c15t.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:33:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-instance.c15t.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:57:33 2026 GMT\n  hsts: null\ndomains:\n- domain: c15t.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n- domain: c15t.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inth/refs/heads/main/security/inth-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consent Management
- Privacy
- Cookie Consent
- GDPR
- CCPA
- Compliance
- Consent
- Developer Tools
- Open Source
---
