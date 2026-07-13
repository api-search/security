---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: owlbot.info
  spf: false
hosts:
- cert_expires: Oct  5 03:58:05 2026 GMT
  host: owlbot.info
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owlbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OwlBot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OwlBot
provider_slug: owlbot
slug: owlbot-domain-security
source_filename: owlbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owlbot.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:58:05 2026 GMT\n  hsts: null\ndomains:\n- domain: owlbot.info\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owlbot/refs/heads/main/security/owlbot-domain-security.yml
summary_line: TLSv1.3
tags:
- Dictionaries
- Public APIs
---
