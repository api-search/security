---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dezhentech.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: dezhentech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dezhentech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dezhentech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dezhentech
provider_slug: dezhentech
slug: dezhentech-domain-security
source_filename: dezhentech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dezhentech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dezhentech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dezhentech/refs/heads/main/security/dezhentech-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Health IT
- Hospital Information Systems
- Electronic Medical Records
- Medical
- Data Integration
- China
---
