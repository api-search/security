---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: latana.com
  spf: true
hosts:
- cert_expires: Oct  1 03:32:31 2026 GMT
  host: www.latana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: app.latana.com
  hsts: false
  https: true
  note: Single-page application shell; answers HTTP 200 with the same 80,361-byte HTML for every path.
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: back.latana.com
  hsts: false
  https: true
  note: 'Rails API backend (REACT_APP_API_URL). /api-docs answers HTTP 401 with a "WWW-Authenticate: Basic" challenge.'
  tls_version: TLSv1.2
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: llmagent.latana.com
  hsts: false
  https: true
  note: '"Data Assistant Streaming Server" (REACT_APP_LLM_AGENT_API_URL); /health returns 200.'
  tls_version: TLSv1.2
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: resources.latana.com
  hsts: false
  https: true
  note: Marketing resources/blog host.
  server: AmazonS3
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Latana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latana, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Latana
provider_slug: latana
slug: latana-domain-security
source_filename: latana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the application hosts discovered in the app.latana.com JavaScript bundle\nnotes: >-\n  The 2026-08-12 pass discovered three Latana-operated hosts that earlier rounds never probed,\n  read from the REACT_APP_* configuration block inside\n  https://app.latana.com/static/js/main.09065b02.chunk.js: back.latana.com (REACT_APP_API_URL,\n  a Rails API backend), llmagent.latana.com (REACT_APP_LLM_AGENT_API_URL, titled \"Data Assistant\n  Streaming Server\") and resources.latana.com. Only the marketing host www.latana.com sends HSTS;\n  the application, API and agent hosts send no Strict-Transport-Security header, and the two\n  backend hosts negotiate TLS 1.2 where the S3-fronted hosts reach TLS 1.3. Recorded as observed.\nhosts:\n- host: www.latana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.latana.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\n  server: AmazonS3\n  note: Single-page application shell; answers HTTP 200 with the same 80,361-byte HTML for every path.\n- host: back.latana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Rails API backend (REACT_APP_API_URL). /api-docs answers HTTP 401 with a\n    \"WWW-Authenticate: Basic\" challenge.\n- host: llmagent.latana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n  note: '\"Data Assistant Streaming Server\" (REACT_APP_LLM_AGENT_API_URL); /health returns 200.'\n- host: resources.latana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\n  server: AmazonS3\n  note: Marketing resources/blog host.\ndomains:\n- domain: latana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latana/refs/heads/main/security/latana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Brand Tracking
- Market Research
- Consumer Insights
- Brand Awareness
- Marketing Analytics
- Survey Data
- Advertising
- Software-as-a-Service
---
