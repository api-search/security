---
api_specs:
- filename: orakl-website-openapi-original.json
  format: json
  label: Orakl Oncology Public Website API
  slug: orakl-oncology-public-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-website-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orakl-oncology.com
  spf: true
hosts:
- cert_expires: Sep 25 19:02:56 2026 GMT
  host: www.orakl-oncology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orakl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orakl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orakl
provider_slug: orakl
slug: orakl-domain-security
source_filename: orakl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orakl-oncology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orakl-oncology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/security/orakl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- TechBio
- Oncology
- Drug Development
- Artificial Intelligence
- Machine Learning
- Healthcare
- Biotechnology
- Precision Medicine
- Cancer Research
- Content Management
- JSON-LD
---
