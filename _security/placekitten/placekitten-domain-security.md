---
api_specs:
- filename: placekitten-openapi.yml
  format: yaml
  label: PlaceKitten
  slug: placekitten
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placekitten/refs/heads/main/openapi/placekitten-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: placekitten.com
  spf: false
hosts:
- cert_expires: Aug 11 20:58:22 2026 GMT
  host: placekitten.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Placekitten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlaceKitten, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PlaceKitten
provider_slug: placekitten
slug: placekitten-domain-security
source_filename: placekitten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placekitten.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 20:58:22 2026 GMT\n  hsts: null\ndomains:\n- domain: placekitten.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placekitten/refs/heads/main/security/placekitten-domain-security.yml
summary_line: TLSv1.3
tags:
- Animals
- Public APIs
- Placeholder
- Images
- Deprecated
---
