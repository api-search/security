---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: secoda.co
  spf: true
hosts:
- cert_expires: Oct  3 21:22:56 2026 GMT
  host: secoda.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secoda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secoda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Secoda
provider_slug: secoda
slug: secoda-domain-security
source_filename: secoda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secoda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:22:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: secoda.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secoda/refs/heads/main/security/secoda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Data Catalog
- Data Governance
- Metadata
- Data Lineage
- Data Quality
- Data Discovery
- Observability
- AI Agents
---
