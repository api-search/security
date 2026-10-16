---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec 10 19:53:50 2026 GMT
  host: cps.sedra-0b3.workers.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cps Cheapest Power Scheduler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CPS (Cheapest-Power Scheduler), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CPS (Cheapest-Power Scheduler)
provider_slug: cps-cheapest-power-scheduler
slug: cps-cheapest-power-scheduler-domain-security
source_filename: cps-cheapest-power-scheduler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cps.sedra-0b3.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 19:53:50 2026 GMT\n  hsts: null\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cps-cheapest-power-scheduler/refs/heads/main/security/cps-cheapest-power-scheduler-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Cloud
- Scheduling
- Optimization
---
