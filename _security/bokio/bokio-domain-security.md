---
api_specs:
- filename: bokio-company-api-openapi.yml
  format: yaml
  label: Bokio Company API
  slug: bokio-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-company-api-openapi.yml
- filename: bokio-general-api-openapi.yml
  format: yaml
  label: Bokio General API
  slug: bokio-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-general-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:security@bokio.se"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bokio.se
  spf: true
hosts:
- cert_expires: Mar 30 15:41:10 2027 GMT
  host: bokio.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.bokio.se
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bokio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bokio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bokio
provider_slug: bokio
slug: bokio-domain-security
source_filename: bokio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bokio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 15:41:10 2027 GMT\n  hsts: false\n- host: api.bokio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bokio.se\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:security@bokio.se\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/security/bokio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Invoicing
- Payments
- Sweden
- SMB
- OAuth
---
