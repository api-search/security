---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activemembrane.com
  spf: true
hosts:
- cert_expires: Nov  3 17:57:30 2026 GMT
  host: www.activemembrane.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Active Membranes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Active Membranes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Active Membranes
provider_slug: active-membranes
slug: active-membranes-domain-security
source_filename: active-membranes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activemembrane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 17:57:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: activemembrane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-membranes/refs/heads/main/security/active-membranes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Water
- Water Technology
- Desalination
- Reverse Osmosis
- Membranes
- Cleantech
- Sustainability
- Industrial
- Hardware
- MCP
- Agents
---
