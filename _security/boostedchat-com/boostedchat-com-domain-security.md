---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boostedchat.com
  spf: true
hosts:
- cert_expires: Jan 20 21:48:56 2027 GMT
  host: boostedchat.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BoostedChat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoostedChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BoostedChat
provider_slug: boostedchat-com
slug: boostedchat-com-domain-security
source_filename: boostedchat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boostedchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 21:48:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: boostedchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/boostedchat-com/security/boostedchat-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Engagement
- Chatbots
- Software-as-a-Service
- Marketing
- E-Commerce
---
