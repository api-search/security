---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laboriq.co
  spf: true
hosts:
- cert_expires: Jan 10 07:27:35 2027 GMT
  host: laboriq.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LaborIQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LaborIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LaborIQ
provider_slug: laboriq-co
slug: laboriq-co-domain-security
source_filename: laboriq-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laboriq.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 07:27:35 2027 GMT\n  hsts: false\ndomains:\n- domain: laboriq.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/laboriq-co/security/laboriq-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Compensation
- Human Resources
- Data Analytics
- Software-as-a-Service
- Workforce
---
