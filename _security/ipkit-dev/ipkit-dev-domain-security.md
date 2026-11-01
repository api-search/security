---
api_specs:
- filename: ipkit-dev-openapi-generated.yml
  format: yaml
  label: IPKit API
  slug: ipkit-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipkit-dev/openapi/_ae-authored/ipkit-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ipkit.dev
  spf: true
hosts:
- cert_expires: Jan  5 05:15:41 2027 GMT
  host: ipkit.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ipkit Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IPKit
provider_slug: ipkit-dev
slug: ipkit-dev-domain-security
source_filename: ipkit-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipkit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:15:41 2027 GMT\n  hsts: false\ndomains:\n- domain: ipkit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ipkit-dev/security/ipkit-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- IP
- Geolocation
- API
- Data
---
