---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: advantumhealth.com
  spf: true
hosts:
- cert_expires: Jan 25 15:49:04 2027 GMT
  host: advantumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advantum Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advantum Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Advantum Health
provider_slug: advantum-health
slug: advantum-health-domain-security
source_filename: advantum-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advantumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 15:49:04 2027 GMT\n  hsts: false\ndomains:\n- domain: advantumhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/advantum-health/security/advantum-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Revenue Cycle Management
- Artificial Intelligence
- Billing
- Coding
---
