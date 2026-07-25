---
api_specs:
- filename: obie-open-data-atm-locator-openapi.json
  format: json
  label: Nationwide ATM Locator API
  slug: nationwide-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-atm-locator-openapi.json
- filename: obie-open-data-branch-locator-openapi.json
  format: json
  label: Nationwide Branch Locator API
  slug: nationwide-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-branch-locator-openapi.json
- filename: obie-open-data-personal-current-accounts-openapi.json
  format: json
  label: Nationwide Personal Current Accounts API
  slug: nationwide-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-personal-current-accounts-openapi.json
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nationwide.co.uk
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.nationwide.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: developer.nationwide.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: openapi.nationwide.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nationwide Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nationwide Building Society, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nationwide Building Society
provider_slug: nationwide-building-society
slug: nationwide-building-society-domain-security
source_filename: nationwide-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nationwide.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nationwide.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\n- host: openapi.nationwide.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nationwide.co.uk\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/security/nationwide-building-society-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
---
