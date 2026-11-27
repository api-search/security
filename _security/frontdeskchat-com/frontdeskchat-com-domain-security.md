---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: frontdeskchat.com
  spf: true
hosts:
- cert_expires: Jan  4 09:44:46 2027 GMT
  host: frontdeskchat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FrontDeskChat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrontDeskChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FrontDeskChat
provider_slug: frontdeskchat-com
slug: frontdeskchat-com-domain-security
source_filename: frontdeskchat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontdeskchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 09:44:46 2027 GMT\n  hsts: false\ndomains:\n- domain: frontdeskchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/frontdeskchat-com/security/frontdeskchat-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Front Desk
- Automation
- Scheduling
- Sales
---
