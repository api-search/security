---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claudeforcompliance.com
  spf: true
hosts:
- cert_expires: Dec 29 15:36:09 2026 GMT
  host: claudeforcompliance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claude for Compliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claude for Compliance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claude for Compliance
provider_slug: claudeforcompliance-com
slug: claudeforcompliance-com-domain-security
source_filename: claudeforcompliance-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claudeforcompliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:36:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claudeforcompliance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/claudeforcompliance-com/security/claudeforcompliance-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mortgage Compliance
- Compliance API
- AI Governance
---
