---
api_specs:
- filename: library-of-congress-loc-gov-json-api-openapi.yml
  format: yaml
  label: Library of Congress loc.gov JSON API
  slug: loc-gov-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-loc-gov-json-api-openapi.yml
- filename: library-of-congress-chronicling-america-api-openapi.yml
  format: yaml
  label: Library of Congress Chronicling America API
  slug: chronicling-america-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-chronicling-america-api-openapi.yml
- filename: library-of-congress-congress-gov-api-openapi.yml
  format: yaml
  label: Library of Congress Congress.gov API
  slug: congress-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-congress-gov-api-openapi.yml
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
- cert_expires: Sep 13 04:56:11 2026 GMT
  host: chroniclingamerica.loc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 11:20:55 2026 GMT
  host: api.congress.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Library Of Congress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Library of Congress, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Library of Congress
provider_slug: library-of-congress
slug: library-of-congress-domain-security
source_filename: library-of-congress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:51:22 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: chroniclingamerica.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:56:11 2026 GMT\n  hsts: null\n- host: api.congress.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: loc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: congress.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/security/library-of-congress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cultural Heritage
- Federal Government
- Library
- Legislative
- Newspapers
- Search
---
