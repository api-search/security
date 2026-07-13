---
api_specs:
- filename: freetogame-openapi.yml
  format: yaml
  label: FreeToGame
  slug: freetogame
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freetogame/refs/heads/main/openapi/freetogame-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freetogame.com
  spf: true
hosts:
- cert_expires: Aug 30 05:05:28 2026 GMT
  host: www.freetogame.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freetogame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeToGame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FreeToGame
provider_slug: freetogame
slug: freetogame-domain-security
source_filename: freetogame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freetogame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:05:28 2026 GMT\n  hsts: null\ndomains:\n- domain: freetogame.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freetogame/refs/heads/main/security/freetogame-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games
- Gaming
---
