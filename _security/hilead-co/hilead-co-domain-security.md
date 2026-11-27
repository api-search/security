---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hilead.co
  spf: true
hosts:
- cert_expires: Dec 30 20:11:40 2026 GMT
  host: hilead.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hilead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hilead
provider_slug: hilead-co
slug: hilead-co-domain-security
source_filename: hilead-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilead.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:11:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hilead.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hilead-co/security/hilead-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Lead Generation
- Email Marketing
- LinkedIn Outreach
- Software-as-a-Service
- Company
---
