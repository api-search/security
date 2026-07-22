---
api_specs:
- filename: qargo-tms-openapi-original.yml
  format: yaml
  label: Qargo TMS API
  slug: qargo-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/openapi/qargo-tms-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: qargo.com
  spf: true
hosts:
- cert_expires: Sep  1 20:45:57 2026 GMT
  host: www.qargo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:57:52 2026 GMT
  host: api-docs.qargo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:14:41 2026 GMT
  host: api.qargo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qargo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Qargo
provider_slug: qargo
slug: qargo-domain-security
source_filename: qargo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:45:57 2026 GMT\n  hsts: false\n- host: api-docs.qargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:57:52 2026 GMT\n  hsts: false\n- host: api.qargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:14:41 2026 GMT\n  hsts: null\ndomains:\n- domain: qargo.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/security/qargo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Transport Management
- Logistics
- Supply Chain
- Freight
- TMS
- Accounting
- Webhooks
---
