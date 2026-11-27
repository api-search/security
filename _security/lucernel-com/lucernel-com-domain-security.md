---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lucernel.com
  spf: true
hosts:
- cert_expires: Feb  7 23:00:26 2027 GMT
  host: lucernel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lucernel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucernel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lucernel
provider_slug: lucernel-com
slug: lucernel-com-domain-security
source_filename: lucernel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:00:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lucernel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lucernel-com/security/lucernel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software-as-a-Service
- iPhone
- Web App
- Independent
- Tools
---
