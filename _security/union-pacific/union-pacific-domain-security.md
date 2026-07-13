---
api_specs:
- filename: union-pacific-api.yaml
  format: yaml
  label: Union Pacific API
  slug: union-pacific
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/union-pacific/refs/heads/main/openapi/union-pacific-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: up.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.up.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.up.com
  https: false
kind: domain-security
layout: security
method: probed
name: Union Pacific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Union Pacific, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Union Pacific
provider_slug: union-pacific
slug: union-pacific-domain-security
source_filename: union-pacific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.up.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: api.up.com\n  https: false\ndomains:\n- domain: up.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/union-pacific/refs/heads/main/security/union-pacific-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
- Freight
- Railroads
- Shipping
- Trains
- Supply Chain
- Logistics
---
