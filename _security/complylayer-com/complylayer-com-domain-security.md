---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: complylayer.com
  spf: true
hosts:
- cert_expires: Dec 12 18:52:23 2026 GMT
  host: complylayer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ComplyLayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComplyLayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ComplyLayer
provider_slug: complylayer-com
slug: complylayer-com-domain-security
source_filename: complylayer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: complylayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:52:23 2026 GMT\n  hsts: false\ndomains:\n- domain: complylayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/complylayer-com/security/complylayer-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Governance
- Compliance
- EU AI Act
- Risk Management
- GDPR
- MCP
- Privacy
---
