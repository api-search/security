---
api_specs:
- filename: loc-loc-gov-json-api-openapi.yml
  format: yaml
  label: loc.gov JSON API
  slug: locgov-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/openapi/loc-loc-gov-json-api-openapi.yml
- filename: loc-congress-gov-openapi.yml
  format: yaml
  label: Congress.gov API
  slug: congressgov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/openapi/loc-congress-gov-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: loc.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: congress.gov
  spf: true
hosts:
- cert_expires: Sep 12 02:51:22 2026 GMT
  host: www.loc.gov
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 11:20:55 2026 GMT
  host: api.congress.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:56:11 2026 GMT
  host: chroniclingamerica.loc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Library of Congress, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Library of Congress
provider_slug: loc
slug: loc-domain-security
source_filename: loc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:51:22 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: api.congress.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:20:55 2026 GMT\n  hsts: null\n- host: chroniclingamerica.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:56:11 2026 GMT\n  hsts: null\ndomains:\n- domain: loc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: congress.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/security/loc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Library
- Government
- Congress
- Legislative Data
- Digital Collections
- Newspapers
- Maps
- Bibliographic Records
- Historical Documents
---
