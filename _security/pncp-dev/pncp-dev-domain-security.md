---
api_specs:
- filename: pncp-dev-openapi-generated.yml
  format: yaml
  label: pncp-dev API
  slug: pncp-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pncp-dev/openapi/_ae-authored/pncp-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pncp.dev
  spf: true
hosts:
- cert_expires: Jan 11 19:25:01 2027 GMT
  host: pncp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pncp Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pncp-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: pncp-dev
provider_slug: pncp-dev
slug: pncp-dev-domain-security
source_filename: pncp-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pncp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 19:25:01 2027 GMT\n  hsts: false\ndomains:\n- domain: pncp.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pncp-dev/security/pncp-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API Proxy
- Public Data
- Brazil
- Procurement
- Open Data
---
