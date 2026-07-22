---
api_specs:
- filename: onshape-openapi-original.json
  format: json
  label: Onshape REST API
  slug: onshape-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/openapi/onshape-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onshape.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: cad.onshape.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onshape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onshape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Onshape
provider_slug: onshape
slug: onshape-domain-security
source_filename: onshape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cad.onshape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: onshape.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/security/onshape-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- CAD
- PLM
- Product Data Management
- Engineering
- Manufacturing
- Design
- Cloud
- Developer Tools
---
