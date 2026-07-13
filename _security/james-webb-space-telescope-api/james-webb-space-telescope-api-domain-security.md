---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jwstapi.com
  spf: false
hosts:
- cert_expires: Aug 12 04:10:59 2026 GMT
  host: jwstapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:15:14 2026 GMT
  host: api.jwstapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: James Webb Space Telescope Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for James Webb Space Telescope API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: James Webb Space Telescope API
provider_slug: james-webb-space-telescope-api
slug: james-webb-space-telescope-api-domain-security
source_filename: james-webb-space-telescope-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jwstapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 04:10:59 2026 GMT\n  hsts: false\n- host: api.jwstapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:15:14 2026 GMT\n  hsts: null\ndomains:\n- domain: jwstapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/james-webb-space-telescope-api/refs/heads/main/security/james-webb-space-telescope-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Astronomy
- JWST
- NASA
- Science
- Space
---
