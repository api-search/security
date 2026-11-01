---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: i95dev.com
  spf: true
hosts:
- cert_expires: Nov 30 06:07:30 2026 GMT
  host: i95dev.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: I95Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for i95Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: i95Dev
provider_slug: i95dev
slug: i95dev-domain-security
source_filename: i95dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: i95dev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 06:07:30 2026 GMT\n  hsts: false\ndomains:\n- domain: i95dev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/i95dev/security/i95dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Integration
- ERP
- Software-as-a-Service
---
