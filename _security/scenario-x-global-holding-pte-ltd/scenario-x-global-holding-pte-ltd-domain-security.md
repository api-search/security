---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scenario-x.ai
  spf: true
hosts:
- cert_expires: Aug 23 20:59:33 2026 GMT
  host: scenario-x.ai
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scenario X Global Holding Pte Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SCENARIO-X GLOBAL HOLDING PTE. LTD., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SCENARIO-X GLOBAL HOLDING PTE. LTD.
provider_slug: scenario-x-global-holding-pte-ltd
slug: scenario-x-global-holding-pte-ltd-domain-security
source_filename: scenario-x-global-holding-pte-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scenario-x.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: scenario-x.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scenario-x-global-holding-pte-ltd/refs/heads/main/security/scenario-x-global-holding-pte-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Financial Services
- Risk Management
- Stress Testing
- Regtech
- Quantum Computing
- Fintech
---
