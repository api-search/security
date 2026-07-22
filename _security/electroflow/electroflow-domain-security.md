---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: eflowtech.com
  spf: true
hosts:
- cert_expires: Sep  2 17:30:39 2026 GMT
  host: www.eflowtech.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electroflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electroflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Electroflow
provider_slug: electroflow
slug: electroflow-domain-security
source_filename: electroflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eflowtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:30:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: eflowtech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electroflow/refs/heads/main/security/electroflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Energy
- Battery Materials
- Lithium
- Clean Technology
- Manufacturing
- Climate Tech
---
