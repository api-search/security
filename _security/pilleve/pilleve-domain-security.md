---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pilleve.com
  spf: true
hosts:
- cert_expires: Oct 13 21:22:40 2026 GMT
  host: pilleve.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pilleve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pilleve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pilleve
provider_slug: pilleve
slug: pilleve-domain-security
source_filename: pilleve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pilleve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 21:22:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: pilleve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pilleve/refs/heads/main/security/pilleve-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Digital Health
- Healthcare
- Medication Adherence
- Controlled Substances
- Patient Monitoring
- Medical Devices
---
