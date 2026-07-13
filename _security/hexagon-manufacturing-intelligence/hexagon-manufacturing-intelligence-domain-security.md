---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hexagon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hexagonmi.com
  spf: false
hosts:
- cert_expires: Aug 17 05:25:15 2026 GMT
  host: hexagon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.hexagonmi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hexagon Manufacturing Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hexagon Manufacturing Intelligence, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hexagon Manufacturing Intelligence
provider_slug: hexagon-manufacturing-intelligence
slug: hexagon-manufacturing-intelligence-domain-security
source_filename: hexagon-manufacturing-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hexagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:25:15 2026 GMT\n  hsts: null\n- host: docs.hexagonmi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hexagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hexagonmi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon-manufacturing-intelligence/refs/heads/main/security/hexagon-manufacturing-intelligence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Manufacturing
- Quality Management
- Metrology
- CAD
- Industrial Automation
- Smart Factory
- Quality Control
---
