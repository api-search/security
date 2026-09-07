---
api_specs:
- filename: 7signalsolutions-openapi.json
  format: json
  label: 7SIGNAL Platform API (Gateway v2)
  slug: 7signal-platform-api-gateway-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/openapi/7signalsolutions-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 7signal.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: 7signal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: api-v2.7signal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: mcp-v2.7signal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 7Signalsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7SIGNAL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 7SIGNAL
provider_slug: 7signalsolutions
slug: 7signalsolutions-domain-security
source_filename: 7signalsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 7signal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v2.7signal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\n- host: mcp-v2.7signal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 7signal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/security/7signalsolutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wireless Network Monitoring
- Wi-Fi Experience Monitoring
- Digital Experience Monitoring
- Network Performance Monitoring
- Network Observability
- AIOps
- IT Operations
- Endpoint Monitoring
- Time Series
- MCP
- agent-native
- Company
---
