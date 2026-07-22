---
api_specs:
- filename: lobcom-openapi-original.yml
  format: yaml
  label: Lob API
  slug: lobcom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lobcom/refs/heads/main/openapi/lobcom-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@lob.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lob.com
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.lob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lobcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lob.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lob.com
provider_slug: lobcom
slug: lobcom-domain-security
source_filename: lobcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.lob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lob.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@lob.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lobcom/refs/heads/main/security/lobcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Direct Mail
- Print
- Address Verification
- Mail
- Postcards
- Letters
- Checks
- Campaigns
- USPS
- Deliverability
---
