---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fpt-is.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: fpt-is.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fpt Is Company Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FPT IS Company Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FPT IS Company Limited
provider_slug: fpt-is-company-limited
slug: fpt-is-company-limited-domain-security
source_filename: fpt-is-company-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fpt-is.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fpt-is.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fpt-is-company-limited/security/fpt-is-company-limited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- IT Services
- Digital Transformation
- Cloud
- AI
---
