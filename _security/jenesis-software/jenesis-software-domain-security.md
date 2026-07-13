---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jenesissoftware.com
  spf: true
hosts:
- cert_expires: Sep 30 04:48:47 2026 GMT
  host: www.jenesissoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jenesis Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jenesis Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jenesis Software
provider_slug: jenesis-software
slug: jenesis-software-domain-security
source_filename: jenesis-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jenesissoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:48:47 2026 GMT\n  hsts: false\ndomains:\n- domain: jenesissoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenesis-software/refs/heads/main/security/jenesis-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Agency Management System
- InsurTech
- Property and Casualty
- Policy Management
- ACORD
- Carrier Downloads
- No Public API
---
