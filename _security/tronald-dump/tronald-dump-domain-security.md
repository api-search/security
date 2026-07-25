---
api_specs:
- filename: tronald-dump-authors-api-openapi.yml
  format: yaml
  label: Tronald Dump Authors API
  slug: tronald-dump-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronald-dump/refs/heads/main/openapi/tronald-dump-authors-api-openapi.yml
- filename: tronald-dump-quotes-api-openapi.yml
  format: yaml
  label: Tronald Dump Quotes API
  slug: tronald-dump-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronald-dump/refs/heads/main/openapi/tronald-dump-quotes-api-openapi.yml
- filename: tronald-dump-sources-api-openapi.yml
  format: yaml
  label: Tronald Dump Sources API
  slug: tronald-dump-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronald-dump/refs/heads/main/openapi/tronald-dump-sources-api-openapi.yml
- filename: tronald-dump-tags-api-openapi.yml
  format: yaml
  label: Tronald Dump Tags API
  slug: tronald-dump-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronald-dump/refs/heads/main/openapi/tronald-dump-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tronalddump.io
  spf: false
hosts:
- cert_expires: Sep 14 22:17:07 2026 GMT
  host: www.tronalddump.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.tronalddump.io
  https: false
kind: domain-security
layout: security
method: probed
name: Tronald Dump Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tronald Dump, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tronald Dump
provider_slug: tronald-dump
slug: tronald-dump-domain-security
source_filename: tronald-dump-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tronalddump.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:17:07 2026 GMT\n  hsts: false\n- host: api.tronalddump.io\n  https: false\ndomains:\n- domain: tronalddump.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronald-dump/refs/heads/main/security/tronald-dump-domain-security.yml
summary_line: TLSv1.3
tags:
- Community
- Games And Comics
- Open Source
- Politics
- Public APIs
- Quotes
- Trump
---
