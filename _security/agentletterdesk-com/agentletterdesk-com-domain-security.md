---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentletterdesk.com
  spf: true
hosts:
- cert_expires: Jan 11 13:32:12 2027 GMT
  host: agentletterdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Letter Desk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Letter Desk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agent Letter Desk
provider_slug: agentletterdesk-com
slug: agentletterdesk-com-domain-security
source_filename: agentletterdesk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentletterdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 13:32:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentletterdesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentletterdesk-com/security/agentletterdesk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Mail
- Certified Mail
- LetterService
- Automation
- Company
---
