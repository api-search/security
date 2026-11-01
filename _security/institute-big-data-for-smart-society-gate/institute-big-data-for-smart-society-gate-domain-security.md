---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gate-ai.eu
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: www.gate-ai.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Institute Big Data For Smart Society Gate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Institute “Big Data for Smart Society” - GATE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Institute “Big Data for Smart Society” - GATE
provider_slug: institute-big-data-for-smart-society-gate
slug: institute-big-data-for-smart-society-gate-domain-security
source_filename: institute-big-data-for-smart-society-gate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gate-ai.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gate-ai.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/institute-big-data-for-smart-society-gate/security/institute-big-data-for-smart-society-gate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Big Data
- Smart Society
- AI
---
