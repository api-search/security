---
api_specs:
- filename: scimar-content-openapi.yml
  format: yaml
  label: Scimar Content API (WordPress REST wp/v2)
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scimar.ca
  spf: true
hosts:
- cert_expires: Nov  1 06:11:23 2026 GMT
  host: scimar.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scimar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scimar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scimar
provider_slug: scimar
slug: scimar-domain-security
source_filename: scimar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scimar.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:11:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scimar.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/security/scimar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Diabetes
- Diagnostics
- Clinical Trials
- Health
- Nutrition
- Research
- Canada
- Content
---
