---
api_specs:
- filename: packagex-openapi-original.yml
  format: yaml
  label: PackageX Shipments API
  slug: packagex-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packagex/refs/heads/main/openapi/packagex-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: packagex.io
  spf: true
hosts:
- cert_expires: Oct  3 01:20:20 2026 GMT
  host: packagex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packagex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PackageX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PackageX
provider_slug: packagex
slug: packagex-domain-security
source_filename: packagex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packagex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:20:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packagex.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packagex/refs/heads/main/security/packagex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Logistics
- Shipping
- Supply Chain
- Computer Vision
- OCR
- Package Tracking
- Fulfillment
---
