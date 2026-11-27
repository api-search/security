---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ebilanzfabrik.de
  spf: true
hosts:
- cert_expires: Dec 13 18:35:55 2026 GMT
  host: ebilanzfabrik.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eBilanz Fabrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eBilanz Fabrik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: eBilanz Fabrik
provider_slug: ebilanzfabrik-de
slug: ebilanzfabrik-de-domain-security
source_filename: ebilanzfabrik-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ebilanzfabrik.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:35:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ebilanzfabrik.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ebilanzfabrik-de/security/ebilanzfabrik-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Accounting
- Tax
- Software-as-a-Service
- Germany
---
