---
api_specs:
- filename: moneyhub-data-api-swagger.json
  format: json
  label: Moneyhub Data & Intelligence API
  slug: moneyhub-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneyhub/refs/heads/main/openapi/moneyhub-data-api-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moneyhub.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: moneyhubenterprise.com
  spf: true
hosts:
- cert_expires: Sep 25 01:38:28 2026 GMT
  host: www.moneyhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:50:51 2026 GMT
  host: docs.moneyhubenterprise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.moneyhub.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moneyhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moneyhub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moneyhub
provider_slug: moneyhub
slug: moneyhub-domain-security
source_filename: moneyhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moneyhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:38:28 2026 GMT\n  hsts: false\n- host: docs.moneyhubenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:50:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moneyhub.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moneyhub.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moneyhubenterprise.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneyhub/refs/heads/main/security/moneyhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- United Kingdom
- Open Banking
- Open Finance
- Account-to-Account
- Payment Initiation
- Data Aggregation
- AISP
- PISP
- Fintech
---
