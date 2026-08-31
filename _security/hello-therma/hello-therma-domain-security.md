---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: glaciergrid.com
  spf: true
hosts:
- cert_expires: Oct 30 09:09:17 2026 GMT
  host: www.glaciergrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: mcp.glaciergrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hello Therma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Therma, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hello Therma
provider_slug: hello-therma
slug: hello-therma-domain-security
source_filename: hello-therma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glaciergrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 09:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.glaciergrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glaciergrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-therma/refs/heads/main/security/hello-therma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Internet of Things
- Energy
- Sustainability
- Cold Chain
- Temperature Monitoring
- Refrigeration
- HVAC
- Building Automation
- Food Safety
- Facilities Management
- Restaurant
- Retail
- MCP
- Agents
---
