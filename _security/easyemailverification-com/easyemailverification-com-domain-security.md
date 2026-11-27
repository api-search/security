---
api_specs:
- filename: easyemailverification-com-account-api-openapi.yml
  format: yaml
  label: Easy Email Verification Account API
  slug: easyemailverification-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-account-api-openapi.yml
- filename: easyemailverification-com-bulk-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Bulk Verification API
  slug: easyemailverification-com-bulk-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-bulk-verification-api-openapi.yml
- filename: easyemailverification-com-single-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Single Verification API
  slug: easyemailverification-com-single-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-single-verification-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easyemailverification.com
  spf: true
hosts:
- cert_expires: Dec 17 22:45:56 2026 GMT
  host: easyemailverification.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easy Email Verification Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easy Email Verification, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Easy Email Verification
provider_slug: easyemailverification-com
slug: easyemailverification-com-domain-security
source_filename: easyemailverification-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easyemailverification.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 22:45:56 2026 GMT\n  hsts: false\ndomains:\n- domain: easyemailverification.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easyemailverification-com/security/easyemailverification-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Verification
- Software-as-a-Service
- Data Validation
- Marketing
---
