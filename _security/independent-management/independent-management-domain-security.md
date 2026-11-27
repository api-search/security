---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: independent.management
  spf: true
hosts:
- cert_expires: Jan 10 06:14:46 2027 GMT
  host: independent.management
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IMW Invoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IMW Invoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IMW Invoice
provider_slug: independent-management
slug: independent-management-domain-security
source_filename: independent-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: independent.management\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:14:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: independent.management\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/independent-management/security/independent-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- Billing
- Time Tracking
- Artificial Intelligence
- Freelancers
---
