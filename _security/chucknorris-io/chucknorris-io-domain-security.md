---
api_specs:
- filename: chucknorris-io-openapi.yml
  format: yaml
  label: Chuck Norris Jokes API
  slug: chuck-norris-jokes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chucknorris-io/refs/heads/main/openapi/chucknorris-io-openapi.yml
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
name: Chucknorris Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chucknorris.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: chucknorris.io
provider_slug: chucknorris-io
slug: chucknorris-io-domain-security
source_filename: chucknorris-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.chucknorris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:24:22 2026 GMT\n  hsts: false\ndomains:\n- domain: chucknorris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chucknorris-io/refs/heads/main/security/chucknorris-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Entertainment
- Jokes
- Chuck Norris
- Open Source
- Public APIs
---
