---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: frontstat.com
  spf: true
hosts:
- cert_expires: Dec 15 19:38:23 2026 GMT
  host: frontstat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FrontStat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrontStat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FrontStat
provider_slug: frontstat-com
slug: frontstat-com-domain-security
source_filename: frontstat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontstat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: frontstat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/frontstat-com/security/frontstat-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Visibility
- Startups
- Analytics
- Platform
- Company
---
