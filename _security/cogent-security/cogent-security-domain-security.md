---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cogentsecurity.com
  spf: false
hosts:
- cert_expires: Nov  1 08:31:59 2026 GMT
  host: www.cogentsecurity.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cogent Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cogent Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cogent Security
provider_slug: cogent-security
slug: cogent-security-domain-security
source_filename: cogent-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cogentsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 08:31:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: cogentsecurity.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogent-security/refs/heads/main/security/cogent-security-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Security
- Government
- Defense
- Intelligence
- Risk Management
- Company
---
