---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: siffletdata.com
  spf: true
hosts:
- cert_expires: Oct 16 07:11:02 2026 GMT
  host: www.siffletdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sifflet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sifflet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sifflet
provider_slug: sifflet
slug: sifflet-domain-security
source_filename: sifflet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siffletdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:11:02 2026 GMT\n  hsts: false\ndomains:\n- domain: siffletdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/security/sifflet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Analytics
- Data Observability
- Data Quality
- Data Catalog
- Data Lineage
- Data Governance
- Monitoring
- Metadata
- AI Agents
---
