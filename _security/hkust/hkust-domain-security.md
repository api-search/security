---
api_specs:
- filename: hkust-path-advisor-openapi.yml
  format: yaml
  label: HKUST Path Advisor API
  slug: path-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/openapi/hkust-path-advisor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ust.hk
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.ust.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 19:05:52 2026 GMT
  host: pathadvisor.ust.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 14:28:47 2027 GMT
  host: hkust.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hkust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong University of Science and Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hong Kong University of Science and Technology
provider_slug: hkust
slug: hkust-domain-security
source_filename: hkust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ust.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: pathadvisor.ust.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:05:52 2026 GMT\n  hsts: false\n- host: hkust.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 14:28:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ust.hk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/security/hkust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Research
- Hong Kong
- China
- Research Data
- Open Data
- Identity Federation
- Course Catalog
- Library
- Smart Campus
- API Gateway
- Wayfinding
---
