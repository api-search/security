---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reltio.com
  spf: true
hosts:
- cert_expires: Sep 28 10:27:39 2026 GMT
  host: www.reltio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reltio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reltio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reltio
provider_slug: reltio
slug: reltio-domain-security
source_filename: reltio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reltio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:27:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: reltio.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reltio/refs/heads/main/security/reltio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Analytics
- Master Data Management
- MDM
- Entity Resolution
- Data Quality
- Data Integration
- AI Agents
- MCP
- SAP
---
