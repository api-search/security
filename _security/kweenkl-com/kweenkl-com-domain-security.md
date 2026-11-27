---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kweenkl.com
  spf: true
hosts:
- cert_expires: Jan  2 21:44:57 2027 GMT
  host: kweenkl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kweenkl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kweenkl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kweenkl
provider_slug: kweenkl-com
slug: kweenkl-com-domain-security
source_filename: kweenkl-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kweenkl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:44:57 2027 GMT\n  hsts: false\ndomains:\n- domain: kweenkl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kweenkl-com/security/kweenkl-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Notification
- AI Agents
- Webhook
- Automation
---
