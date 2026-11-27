---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: controldrill.com
  spf: true
hosts:
- cert_expires: Dec 24 00:27:10 2026 GMT
  host: controldrill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ControlDrill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ControlDrill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ControlDrill
provider_slug: controldrill-com
slug: controldrill-com-domain-security
source_filename: controldrill-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: controldrill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 00:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: controldrill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/controldrill-com/security/controldrill-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Incident Response
- Tabletop Exercises
- Compliance
- Security
- SOC 2
- Audit Evidence
- MCP
---
