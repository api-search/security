---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crusoe.ai
  spf: true
hosts:
- cert_expires: Dec 22 17:29:09 2026 GMT
  host: www.crusoe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crusoeenergysystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crusoeenergysystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crusoeenergysystems
provider_slug: crusoeenergysystems
slug: crusoeenergysystems-domain-security
source_filename: crusoeenergysystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crusoe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 17:29:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crusoe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crusoeenergysystems/refs/heads/main/security/crusoeenergysystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Cloud
- Sustainable
- DataCenters
---
