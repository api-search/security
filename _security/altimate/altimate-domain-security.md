---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: altimate.ai
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: altimate.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altimate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altimate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Altimate
provider_slug: altimate
slug: altimate-domain-security
source_filename: altimate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altimate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: altimate.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altimate/refs/heads/main/security/altimate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Engineering
- Artificial Intelligence
- Agents
- dbt
- Data Governance
- MCP
- Developer Tools
- Analytics
---
