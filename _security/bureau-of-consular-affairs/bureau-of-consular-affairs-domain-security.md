---
api_specs:
- filename: bureau-of-consular-affairs-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Data Catalog (CKAN API)
  slug: ca-data-catalog-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: state.gov
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: travel.state.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 13:45:14 2026 GMT
  host: cadatacatalog.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Consular Affairs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Consular Affairs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Consular Affairs
provider_slug: bureau-of-consular-affairs
slug: bureau-of-consular-affairs-domain-security
source_filename: bureau-of-consular-affairs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: travel.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cadatacatalog.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:45:14 2026 GMT\n  hsts: null\ndomains:\n- domain: state.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/security/bureau-of-consular-affairs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Passports
- Travel
- Travel Advisories
- Visas
---
