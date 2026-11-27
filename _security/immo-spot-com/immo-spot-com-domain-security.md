---
api_specs:
- filename: immo-spot-com-api-openapi.yml
  format: yaml
  label: Immo Spot API API
  slug: immo-spot-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immo-spot-com/openapi/_original/immo-spot-com-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: immo-spot.com
  spf: false
hosts:
- cert_expires: Jan 19 23:48:44 2027 GMT
  host: immo-spot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: immo-spot-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for immo-spot-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: immo-spot-com
provider_slug: immo-spot-com
slug: immo-spot-com-domain-security
source_filename: immo-spot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immo-spot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:48:44 2027 GMT\n  hsts: false\ndomains:\n- domain: immo-spot.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/immo-spot-com/security/immo-spot-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
