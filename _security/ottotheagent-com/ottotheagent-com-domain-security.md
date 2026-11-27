---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ottotheagent.com
  spf: true
hosts:
- cert_expires: Jan 25 02:27:56 2027 GMT
  host: ottotheagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otto
provider_slug: ottotheagent-com
slug: ottotheagent-com-domain-security
source_filename: ottotheagent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ottotheagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 02:27:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ottotheagent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ottotheagent-com/security/ottotheagent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Artificial Intelligence
- Software-as-a-Service
- Business Travel
- Automation
- Company
---
