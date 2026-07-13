---
api_specs:
- filename: bloom-credit-api-openapi.yaml
  format: yaml
  label: Bloom Credit API
  slug: bloom-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/openapi/bloom-credit-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bloomcredit.io
  spf: true
hosts:
- cert_expires: Sep 13 07:57:17 2026 GMT
  host: bloomcredit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 02:59:49 2026 GMT
  host: api.bloomcredit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.sandbox.bloomcredit.io
  https: false
kind: domain-security
layout: security
method: probed
name: Bloom Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloom Credit, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bloom Credit
provider_slug: bloom-credit
slug: bloom-credit-domain-security
source_filename: bloom-credit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomcredit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bloomcredit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:59:49 2026 GMT\n  hsts: null\n- host: api.sandbox.bloomcredit.io\n  https: false\ndomains:\n- domain: bloomcredit.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/security/bloom-credit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
---
