---
api_specs:
- filename: usemip-openapi-generated.yml
  format: yaml
  label: usemip.com API
  slug: usemip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usemip/openapi/_ae-authored/usemip-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: usemip.com
  spf: true
hosts:
- cert_expires: Nov 29 16:40:21 2026 GMT
  host: usemip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usemip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for usemip.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: usemip.com
provider_slug: usemip
slug: usemip-domain-security
source_filename: usemip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usemip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 16:40:21 2026 GMT\n  hsts: false\ndomains:\n- domain: usemip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/usemip/security/usemip-domain-security.yml
summary_line: TLSv1.3
tags:
- Integration
- Artificial Intelligence
- Data
- Platform
- Hybrid
---
