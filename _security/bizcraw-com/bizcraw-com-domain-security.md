---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bizcraw.com
  spf: false
hosts:
- cert_expires: Dec 31 07:17:12 2026 GMT
  host: bizcraw.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bizcraw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizcraw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bizcraw
provider_slug: bizcraw-com
slug: bizcraw-com-domain-security
source_filename: bizcraw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bizcraw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bizcraw.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bizcraw-com/security/bizcraw-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Scraping
- AI Sales
- Lead Generation
- CRM Integration
- Software-as-a-Service
- Automation
---
