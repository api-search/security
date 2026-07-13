---
api_specs:
- filename: openapi.json
  format: json
  label: Giant Bomb API
  slug: giantbomb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: giantbomb.com
  spf: true
hosts:
- cert_expires: Aug 26 00:14:39 2026 GMT
  host: www.giantbomb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Giantbomb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giant Bomb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Giant Bomb
provider_slug: giantbomb
slug: giantbomb-domain-security
source_filename: giantbomb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.giantbomb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:14:39 2026 GMT\n  hsts: null\ndomains:\n- domain: giantbomb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/security/giantbomb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Entertainment
- Video Games
- Game Database
- Gaming
- Media
---
