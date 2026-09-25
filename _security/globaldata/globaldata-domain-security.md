---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: globaldata.com
  spf: true
hosts:
- cert_expires: Feb 27 14:22:01 2027 GMT
  host: www.globaldata.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: mcp.globaldata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Globaldata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlobalData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GlobalData
provider_slug: globaldata
slug: globaldata-domain-security
source_filename: globaldata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globaldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 14:22:01 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: mcp.globaldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: globaldata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldata/refs/heads/main/security/globaldata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Intelligence
- Business Intelligence
- Data
- Analytics
- MCP
- Agents
- Company Data
- Deals
- News
- Patents
- Research
- Financial Services
- Energy
- Mining
---
