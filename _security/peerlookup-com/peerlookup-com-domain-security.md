---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: peerlookup.com
  spf: true
hosts:
- cert_expires: Dec 18 18:09:34 2026 GMT
  host: peerlookup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peerlookup Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for peerlookup-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: peerlookup-com
provider_slug: peerlookup-com
slug: peerlookup-com-domain-security
source_filename: peerlookup-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peerlookup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 18:09:34 2026 GMT\n  hsts: false\ndomains:\n- domain: peerlookup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/peerlookup-com/security/peerlookup-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Public API
- MCP
- Knowledge Sharing
- Open Data
- Board
---
