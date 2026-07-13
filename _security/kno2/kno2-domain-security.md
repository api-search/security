---
api_specs:
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Messaging API
  slug: kno2-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Intake and Retrieval API
  slug: kno2-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Directory API
  slug: kno2-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kno2.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com a:zgateway.zuora.com include:spf.mail.intercom.io include:44204548.spf02.hubspotemail.net -all
hosts:
- cert_expires: Sep 24 22:02:21 2026 GMT
  cert_issuer: Let's Encrypt (YE2)
  host: kno2.com
  hsts: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 6 03:58:44 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: app.kno2fy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:27:48 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: developer.kno2.com
  hsts: true
  hsts_max_age: 31536000
  http_status: 302
  https: true
  note: Redirects to OAuth login (ReadMe-hosted developer portal).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kno2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kno2, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kno2
provider_slug: kno2
slug: kno2-domain-security
source_filename: kno2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of Kno2 web, app, and developer hosts\nnotes: >-\n  The production Communication API runs on per-subscription tenant hosts under\n  kno2fy.com (e.g. {subscription}.kno2fy.com) which are not publicly probeable\n  without a provisioned subscription. Probes below cover the public marketing\n  site, the Kno2fy application host, and the developer portal.\nhosts:\n- host: kno2.com\n  https: true\n  http_status: 200\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE2)\n  cert_expires: Sep 24 22:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.kno2fy.com\n  https: true\n  http_status: 200\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 6 03:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n- host: developer.kno2.com\n  https: true\n  http_status: 302\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services\
  \ (WE1)\n  cert_expires: Sep 23 05:27:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Redirects to OAuth login (ReadMe-hosted developer portal).\ndomains:\n- domain: kno2.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com a:zgateway.zuora.com include:spf.mail.intercom.io include:44204548.spf02.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/security/kno2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
