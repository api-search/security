---
api_specs:
- filename: neighbortunes-openapi.yml
  format: yaml
  label: Neighbortunes
  slug: neighbortunes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neighbortunes.net
  spf: true
hosts:
- cert_expires: Sep  1 04:18:10 2026 GMT
  host: www.neighbortunes.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:18:10 2026 GMT
  host: neighbortunes.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neighbortunes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neighbortunes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neighbortunes
provider_slug: neighbortunes
slug: neighbortunes-domain-security
source_filename: neighbortunes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neighbortunes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:18:10 2026 GMT\n  hsts: false\n- host: neighbortunes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:18:10 2026 GMT\n  hsts: false\ndomains:\n- domain: neighbortunes.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/security/neighbortunes-domain-security.yml
summary_line: TLSv1.3
tags:
- Music
- Setlists
- Fan Site
---
