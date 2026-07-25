---
api_specs:
- filename: obie-open-data-openapi.json
  format: json
  label: TSB Open Data API
  slug: tsb-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/obie-open-data-openapi.json
- filename: tsb-bank-oauth-server-openapi.json
  format: json
  label: TSB OAuth Toolkit (OTK) Server
  slug: tsb-oauth-toolkit-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-oauth-server-openapi.json
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tsb.co.uk
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.tsb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: apis.tsb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: apis.developer.tsb.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsb Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TSB Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TSB Bank
provider_slug: tsb-bank
slug: tsb-bank-domain-security
source_filename: tsb-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: apis.tsb.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: apis.developer.tsb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tsb.co.uk\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/security/tsb-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech
---
