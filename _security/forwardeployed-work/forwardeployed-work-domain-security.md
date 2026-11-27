---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: forwardeployed.work
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cerebrixos.com
  spf: true
hosts:
- cert_expires: Jan 17 17:00:16 2027 GMT
  host: forwardeployed.work
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 15:51:56 2027 GMT
  host: cerebrixos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: CerebrixOS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CerebrixOS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CerebrixOS
provider_slug: forwardeployed-work
slug: forwardeployed-work-domain-security
source_filename: forwardeployed-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forwardeployed.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 17:00:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cerebrixos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 15:51:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: forwardeployed.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cerebrixos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/forwardeployed-work/security/forwardeployed-work-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Workforce
- Process Diagnostic
- AI Process Audit
- Simulation
- Judgement as a Service
- Embedded Support
- Watchtower
- Sovereign Log Analysis
---
