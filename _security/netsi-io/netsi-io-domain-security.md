---
api_specs:
- filename: netsi-io-api-openapi.json
  format: json
  label: netsi API API
  slug: netsi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netsi-io/openapi/_original/netsi-io-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: netsi.io
  spf: true
hosts:
- cert_expires: Jan 15 23:27:09 2027 GMT
  host: netsi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: netsi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for netsi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: netsi
provider_slug: netsi-io
slug: netsi-io-domain-security
source_filename: netsi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netsi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:27:09 2027 GMT\n  hsts: false\ndomains:\n- domain: netsi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/netsi-io/security/netsi-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Personal
- Networks
- Agents
- Privacy
- Open Source
---
