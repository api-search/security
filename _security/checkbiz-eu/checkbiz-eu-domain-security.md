---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkbiz.eu
  spf: true
hosts:
- cert_expires: Jan 26 07:02:14 2027 GMT
  host: checkbiz.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 04:24:07 2027 GMT
  host: platform.checkbiz.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 07:25:48 2027 GMT
  host: api.checkbiz.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: CheckBiz.eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CheckBiz.eu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CheckBiz.eu
provider_slug: checkbiz-eu
slug: checkbiz-eu-domain-security
source_filename: checkbiz-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: checkbiz.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 07:02:14 2027 GMT\n  hsts: false\n- host: platform.checkbiz.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 04:24:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.checkbiz.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:25:48 2027 GMT\n  hsts: null\ndomains:\n- domain: checkbiz.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/checkbiz-eu/security/checkbiz-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Company Verification
- Business Registers
- VAT
- Brand Protection
- Fraud Prevention
- E-Commerce
- AI Agents
- MCP
- Europe
---
