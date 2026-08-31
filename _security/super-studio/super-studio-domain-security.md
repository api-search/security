---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: super-studio.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ec-force.com
  spf: true
hosts:
- cert_expires: Oct 14 23:52:48 2026 GMT
  host: www.super-studio.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: apidoc.ec-force.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:22:28 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SUPER STUDIO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SUPER STUDIO
provider_slug: super-studio
slug: super-studio-domain-security
source_filename: super-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.super-studio.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidoc.ec-force.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:22:28 2026 GMT\n  hsts: null\ndomains:\n- domain: super-studio.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ec-force.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-studio/refs/heads/main/security/super-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Commerce
- Subscription Commerce
- Order Management
- Marketing Automation
- Business Intelligence
- Software-as-a-Service
- Artificial Intelligence
- Agents
- MCP
- Japan
---
