---
api_specs:
- filename: naic-content-jsonapi-openapi.yml
  format: yaml
  label: NAIC Content JSON:API
  slug: content-jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/naic/refs/heads/main/openapi/naic-content-jsonapi-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: naic.org
  spf: true
- caa:
  - 0 Issue "amazonaws.com"
  - 0 Issue "globalsign.com"
  dmarc: false
  dnssec: false
  domain: serff.com
  spf: true
hosts:
- cert_expires: Oct  1 12:37:15 2026 GMT
  host: content.naic.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.serff.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: sbs.naic.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Naic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NAIC, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NAIC
provider_slug: naic
slug: naic-domain-security
source_filename: naic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: content.naic.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.serff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\n- host: sbs.naic.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: naic.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: serff.com\n  dnssec: false\n  caa:\n  - 0 Issue \"amazonaws.com\"\n  - 0 Issue \"globalsign.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naic/refs/heads/main/security/naic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Regulator
- Market Infrastructure
- Insurance Regulation
- Property and Casualty
- Life Insurance
- Health Insurance
- Producer Licensing
- Rate and Form Filing
- Regulatory Reporting
- Standards Body
- Model Laws
- Regulatory Data
- Open Data
---
