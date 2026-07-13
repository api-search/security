---
api_specs:
- filename: huntington-bank-treasury-management-api-openapi.yml
  format: yaml
  label: Huntington Bank Treasury Management API
  slug: treasury-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntington-bancshares/refs/heads/main/openapi/huntington-bank-treasury-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huntington.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: hnbdevportal.huntington.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.huntington.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.huntington.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Huntington Bancshares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huntington Bancshares, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huntington Bancshares
provider_slug: huntington-bancshares
slug: huntington-bancshares-domain-security
source_filename: huntington-bancshares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hnbdevportal.huntington.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: www.huntington.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.huntington.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: huntington.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntington-bancshares/refs/heads/main/security/huntington-bancshares-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- ERP Integration
- Open Banking
- Payments
- Treasury
- Fortune 1000
---
