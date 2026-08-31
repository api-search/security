---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: desaisiv.com
  spf: true
hosts:
- cert_expires: Sep 16 18:05:36 2026 GMT
  host: desaisiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Desaisiv Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Desaisiv Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Desaisiv Inc.
provider_slug: desaisiv-inc
slug: desaisiv-inc-domain-security
source_filename: desaisiv-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desaisiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:05:36 2026 GMT\n  hsts: null\ndomains:\n- domain: desaisiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desaisiv-inc/refs/heads/main/security/desaisiv-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- InsurTech
- Insurance
- Health Insurance
- Underwriting
- Claims Automation
- Artificial Intelligence
- Saudi Arabia
- MENA
---
