---
api_specs:
- filename: apigen-apigen-openapi.yml
  format: yaml
  label: APIGen
  slug: apigen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/openapi/apigen-apigen-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apigen.com
  spf: true
hosts:
- cert_expires: Sep 11 00:32:27 2026 GMT
  host: api.apigen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apigen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIGen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIGen
provider_slug: apigen
slug: apigen-domain-security
source_filename: apigen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.apigen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:32:27 2026 GMT\n  hsts: null\ndomains:\n- domain: apigen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/security/apigen-domain-security.yml
summary_line: TLSv1.3
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
---
