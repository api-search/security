---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: davosalestax.com
  spf: true
hosts:
- cert_expires: Jan 24 21:52:17 2027 GMT
  host: davosalestax.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DAVO Sales Tax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAVO Sales Tax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DAVO Sales Tax
provider_slug: davosalestax-com
slug: davosalestax-com-domain-security
source_filename: davosalestax-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: davosalestax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 21:52:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: davosalestax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/davosalestax-com/security/davosalestax-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Tax
- Automation
- Small Business
- Avalara
- Integration
---
