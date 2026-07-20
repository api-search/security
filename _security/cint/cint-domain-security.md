---
api_specs:
- filename: cint-demand-openapi.yml
  format: yaml
  label: Cint Exchange Demand API
  slug: cint-exchange-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cint/refs/heads/main/openapi/cint-demand-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:domains@cint.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cint.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.cint.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cint
provider_slug: cint
slug: cint-domain-security
source_filename: cint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cint.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:domains@cint.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cint/refs/heads/main/security/cint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Market Research
- Survey Sample
- Consumer Insights
- Data Collection
- Ad Measurement
- Marketplace
- Panel
---
