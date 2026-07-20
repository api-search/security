---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ascend.io
  spf: true
hosts:
- cert_expires: Sep 20 18:34:33 2026 GMT
  host: www.ascend.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ascendio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ascend.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ascend.io
provider_slug: ascendio
slug: ascendio-domain-security
source_filename: ascendio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ascend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:34:33 2026 GMT\n  hsts: false\ndomains:\n- domain: ascend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascendio/refs/heads/main/security/ascendio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Big Data
- Data Engineering
- Data Pipelines
- ETL
- Orchestration
- Data Automation
- MCP
- Developer Tools
---
