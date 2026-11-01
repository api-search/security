---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: joinwarp.com
  spf: true
hosts:
- cert_expires: Dec 24 06:46:20 2026 GMT
  host: www.joinwarp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joinwarp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Warp
provider_slug: joinwarp-com
slug: joinwarp-com-domain-security
source_filename: joinwarp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinwarp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 06:46:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinwarp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/joinwarp-com/security/joinwarp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payroll
- Benefits
- Tax Compliance
- IT Management
- Global Payroll
- HRIS
- AI Agents
---
