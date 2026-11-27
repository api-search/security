---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aianyone.com
  spf: true
hosts:
- cert_expires: Jan 11 06:00:29 2027 GMT
  host: aianyone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Anyone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Anyone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AI Anyone
provider_slug: aianyone-com
slug: aianyone-com-domain-security
source_filename: aianyone-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aianyone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 06:00:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aianyone.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aianyone-com/security/aianyone-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Chatbots
- Voice
- Education
- Platform
---
