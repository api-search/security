---
api_specs:
- filename: openapi.json
  format: json
  label: Chuck Norris API
  slug: chuck-norris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chuck-norris/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chucknorris.io
  spf: true
hosts:
- cert_expires: Aug 31 11:24:22 2026 GMT
  host: api.chucknorris.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chuck Norris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chuck Norris API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chuck Norris API
provider_slug: chuck-norris
slug: chuck-norris-domain-security
source_filename: chuck-norris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.chucknorris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:24:22 2026 GMT\n  hsts: false\ndomains:\n- domain: chucknorris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chuck-norris/refs/heads/main/security/chuck-norris-domain-security.yml
summary_line: TLSv1.3
tags:
- Jokes
- Humor
- Entertainment
- Chuck Norris
- Free
---
