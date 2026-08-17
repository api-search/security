---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: warmly.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getwarmly.com
  spf: true
hosts:
- cert_expires: Nov  2 23:06:40 2026 GMT
  host: warmly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 03:16:14 2026 GMT
  host: help.warmly.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:25:12 2026 GMT
  host: opps-api.getwarmly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warmly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warmly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Warmly
provider_slug: warmly
slug: warmly-domain-security
source_filename: warmly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: warmly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:06:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.warmly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:16:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: opps-api.getwarmly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:25:12 2026 GMT\n  hsts: null\ndomains:\n- domain: warmly.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getwarmly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warmly/refs/heads/main/security/warmly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- Marketing
- Intent Data
- Revenue Orchestration
- Website Visitor Identification
- AI Agents
- Go To Market
- MCP
- Lead Generation
- CRM
---
