---
api_specs:
- filename: apiman-openapi.json
  format: json
  label: Apiman
  slug: apiman
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiman.io
  spf: true
hosts:
- cert_expires: Sep 20 19:26:22 2026 GMT
  host: www.apiman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apiman
provider_slug: apiman
slug: apiman-domain-security
source_filename: apiman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:26:22 2026 GMT\n  hsts: false\ndomains:\n- domain: apiman.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/security/apiman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
---
