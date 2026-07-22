---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sheet.rocks
  spf: false
hosts:
- cert_expires: Oct 15 13:37:39 2026 GMT
  host: sheet.rocks
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sheetrocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SheetRocks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: SheetRocks
provider_slug: sheetrocks
slug: sheetrocks-domain-security
source_filename: sheetrocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sheet.rocks\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:37:39 2026 GMT\n  hsts: false\ndomains:\n- domain: sheet.rocks\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheetrocks/refs/heads/main/security/sheetrocks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spreadsheet
- No-Code
- Workflow Automation
- Salesforce
- Embedded Analytics
- Business Applications
---
