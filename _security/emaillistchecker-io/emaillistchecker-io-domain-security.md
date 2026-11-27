---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emaillistchecker.io
  spf: true
hosts:
- cert_expires: Jan 28 18:18:00 2027 GMT
  host: emaillistchecker.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EmailListChecker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailListChecker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EmailListChecker
provider_slug: emaillistchecker-io
slug: emaillistchecker-io-domain-security
source_filename: emaillistchecker-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emaillistchecker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 18:18:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emaillistchecker.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/emaillistchecker-io/security/emaillistchecker-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- Artificial Intelligence
- Software-as-a-Service
- Data Cleaning
- Bulk Verification
- Company
---
