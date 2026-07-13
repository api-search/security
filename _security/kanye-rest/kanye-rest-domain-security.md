---
api_specs:
- filename: kanye-rest-openapi.yml
  format: yaml
  label: kanye.rest
  slug: kanyerest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanye-rest/refs/heads/main/openapi/kanye-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kanye.rest
  spf: true
hosts:
- cert_expires: Sep 14 13:53:01 2026 GMT
  host: kanye.rest
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:39:25 2026 GMT
  host: api.kanye.rest
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kanye Rest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kanye.rest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: kanye.rest
provider_slug: kanye-rest
slug: kanye-rest-domain-security
source_filename: kanye-rest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kanye.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:53:01 2026 GMT\n  hsts: false\n- host: api.kanye.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:39:25 2026 GMT\n  hsts: false\ndomains:\n- domain: kanye.rest\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanye-rest/refs/heads/main/security/kanye-rest-domain-security.yml
summary_line: TLSv1.3
tags:
- Personality
- Quotes
- Open Source
- Cloudflare Workers
- Public APIs
---
