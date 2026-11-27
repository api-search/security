---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rezolve.com
  spf: true
hosts:
- cert_expires: Feb  2 04:23:41 2027 GMT
  host: rezolve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rezolve AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rezolve AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rezolve AI
provider_slug: crownpeak
slug: crownpeak-domain-security
source_filename: crownpeak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rezolve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 04:23:41 2027 GMT\n  hsts: false\ndomains:\n- domain: rezolve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/crownpeak/security/crownpeak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Infrastructure
- Commerce
- Discovery AI
- Conversational AI
- Payments
- Loyalty
- Data Intelligence
---
