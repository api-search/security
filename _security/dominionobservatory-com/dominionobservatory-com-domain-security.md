---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dominionobservatory.com
  spf: true
hosts:
- cert_expires: Dec 17 21:15:14 2026 GMT
  host: dominionobservatory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dominion Observatory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dominion Observatory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dominion Observatory
provider_slug: dominionobservatory-com
slug: dominionobservatory-com-domain-security
source_filename: dominionobservatory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dominionobservatory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 21:15:14 2026 GMT\n  hsts: false\ndomains:\n- domain: dominionobservatory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dominionobservatory-com/security/dominionobservatory-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- MCP
- Trust
- Monitoring
- Compliance
- Gateways
---
