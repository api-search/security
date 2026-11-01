---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: douxprocess.com
  spf: true
hosts:
- cert_expires: Jan 11 22:28:54 2027 GMT
  host: douxprocess.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Douxprocess Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for douxprocess-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: douxprocess-com
provider_slug: douxprocess-com
slug: douxprocess-com-domain-security
source_filename: douxprocess-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: douxprocess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:28:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: douxprocess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/douxprocess-com/security/douxprocess-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Automation
- AI
- SaaS
- Workflow
---
