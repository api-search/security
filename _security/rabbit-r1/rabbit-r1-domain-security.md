---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rabbit.tech
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: www.rabbit.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rabbit R1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rabbit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rabbit
provider_slug: rabbit-r1
slug: rabbit-r1-domain-security
source_filename: rabbit-r1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rabbit.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rabbit.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabbit-r1/refs/heads/main/security/rabbit-r1-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Hardware
- Handheld
- Large Action Model
- LAM
- Agents
- Consumer
- rabbitOS
- Teenage Engineering
---
