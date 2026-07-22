---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clify.co.kr
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: clify.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simpatico Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simpatico Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simpatico Project
provider_slug: simpatico-project
slug: simpatico-project-domain-security
source_filename: simpatico-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clify.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clify.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpatico-project/refs/heads/main/security/simpatico-project-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mental Health
- Wellness
- Employee Assistance Program
- EAP
- Human Resources
- HR Tech
- Artificial Intelligence
- Digital Health
- South Korea
---
