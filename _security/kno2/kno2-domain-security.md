---
api_specs:
- filename: kno2-attachments-api-openapi.yml
  format: yaml
  label: Kno2 Attachments API
  slug: kno2-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-attachments-api-openapi.yml
- filename: kno2-authentication-api-openapi.yml
  format: yaml
  label: Kno2 Authentication API
  slug: kno2-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-authentication-api-openapi.yml
- filename: kno2-directory-api-openapi.yml
  format: yaml
  label: Kno2 Directory API
  slug: kno2-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-directory-api-openapi.yml
- filename: kno2-intake-api-openapi.yml
  format: yaml
  label: Kno2 Intake API
  slug: kno2-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-intake-api-openapi.yml
- filename: kno2-messaging-api-openapi.yml
  format: yaml
  label: Kno2 Messaging API
  slug: kno2-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-messaging-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kno2.com
  spf: true
hosts:
- cert_expires: Sep 24 22:02:21 2026 GMT
  host: kno2.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:27:48 2026 GMT
  host: developer.kno2.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kno2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kno2, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kno2
provider_slug: kno2
slug: kno2-domain-security
source_filename: kno2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kno2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.kno2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:27:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: kno2.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/security/kno2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare Interoperability
- Clinical Records
- Health Information Exchange
- Direct Secure Messaging
- FHIR
- Clinical Documents
- Patient Records
- Healthcare
- HIE
- Care Coordination
- QHIN
- TEFCA
- Carequality
---
