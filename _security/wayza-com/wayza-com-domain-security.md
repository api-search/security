---
api_specs:
- filename: wayza-com-wayza-openapi.json
  format: json
  label: Wayza API
  slug: wayza-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wayza-com/openapi/_original/wayza-com-wayza-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wayza.com
  spf: true
hosts:
- cert_expires: Dec 31 19:56:08 2026 GMT
  host: wayza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wayza Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wayza-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: wayza-com
provider_slug: wayza-com
slug: wayza-com-domain-security
source_filename: wayza-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:56:08 2026 GMT\n  hsts: false\ndomains:\n- domain: wayza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/wayza-com/security/wayza-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Integration
- Protocol
- Open-Source
---
