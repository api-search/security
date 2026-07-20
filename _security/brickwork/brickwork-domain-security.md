---
api_specs:
- filename: brickwork-openapi.yml
  format: yaml
  label: Brickwork API v3
  slug: brickwork-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brickwork/refs/heads/main/openapi/brickwork-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brickworksoftware.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: production.brickworksoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brickwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brickwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brickwork
provider_slug: brickwork
slug: brickwork-domain-security
source_filename: brickwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: production.brickworksoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: brickworksoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brickwork/refs/heads/main/security/brickwork-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Retail
- Omnichannel
- Store Locator
- Appointments
- Events
- Location Data
- CMS
---
