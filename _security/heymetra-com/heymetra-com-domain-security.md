---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heymetra.com
  spf: true
hosts:
- cert_expires: Dec 23 15:00:39 2026 GMT
  host: heymetra.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HeyMetra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyMetra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HeyMetra
provider_slug: heymetra-com
slug: heymetra-com-domain-security
source_filename: heymetra-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heymetra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 15:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: heymetra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/heymetra-com/security/heymetra-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Assistant
- Connectors
- E-Commerce
- Marketing
- Sales
- Analytics
- Agencies
---
