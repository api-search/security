---
api_specs:
- filename: commure-auth-api-openapi.yml
  format: yaml
  label: Commure Auth API
  slug: commure-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/openapi/commure-auth-api-openapi.yml
- filename: commure-fhir-api-openapi.yml
  format: yaml
  label: Commure FHIR API
  slug: commure-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/openapi/commure-fhir-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:ops+caa@commure.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: commure.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
hosts:
- cert_expires: Oct  1 04:57:30 2026 GMT
  host: www.commure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 09:01:44 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commure, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Commure
provider_slug: commure
slug: commure-domain-security
source_filename: commure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:57:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:01:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commure.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:ops+caa@commure.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"\
  pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/security/commure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Clinical AI
- Ambient AI
- Revenue Cycle Management
- FHIR
- SMART on FHIR
- Interoperability
- EHR
- Remote Monitoring
- Health System
- Terminology Services
---
