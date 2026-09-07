---
api_specs:
- filename: openapi.json
  format: json
  label: DomScan API
  slug: domscan-api
  spec_type: OpenAPI
  url: https://domscan.net/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domscan.net
  spf: true
hosts:
- cert_expires: Nov 26 18:28:48 2026 GMT
  host: domscan.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomScan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DomScan
provider_slug: domscan
slug: domscan-domain-security
source_filename: domscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domscan.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:28:48 2026 GMT\n  hsts: null\ndomains:\n- domain: domscan.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domscan/refs/heads/main/security/domscan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Domains
- DNS
- WHOIS
- rdap
- SSL/TLS
- Email Security
- domain-valuation
- Brand Protection
- OSINT
- Threat Intelligence
- MCP
- agent-native
---
