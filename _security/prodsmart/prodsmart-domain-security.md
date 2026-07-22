---
api_specs:
- filename: prodsmart-v1-openapi.yml
  format: yaml
  label: Autodesk Fusion Operations (Prodsmart) API v1
  slug: autodesk-fusion-operations-prodsmart-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prodsmart.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: prodsmart.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prodsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prodsmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prodsmart
provider_slug: prodsmart
slug: prodsmart-domain-security
source_filename: prodsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prodsmart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: prodsmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/security/prodsmart-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Manufacturing
- Manufacturing Execution System
- Production Management
- Inventory
- Shop Floor
- Autodesk
- Industry 4.0
---
