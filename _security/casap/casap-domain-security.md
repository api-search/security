---
api_specs:
- filename: casap-openapi.json
  format: json
  label: Casap API
  slug: casap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casap/refs/heads/main/openapi/casap-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: casaphq.com
  spf: true
hosts:
- cert_expires: Sep 12 19:59:15 2026 GMT
  host: www.casaphq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:51:34 2026 GMT
  host: docs.casaphq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:11:15 2026 GMT
  host: api.casaphq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Casap
provider_slug: casap
slug: casap-domain-security
source_filename: casap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.casaphq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.casaphq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:51:34 2026 GMT\n  hsts: false\n- host: api.casaphq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:11:15 2026 GMT\n  hsts: null\ndomains:\n- domain: casaphq.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casap/refs/heads/main/security/casap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Disputes
- Chargebacks
- Fraud
- Payments
- Banking
- Dispute Resolution
- Agentic AI
---
