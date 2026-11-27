---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixidu.com
  spf: true
hosts:
- cert_expires: Dec 19 22:17:39 2026 GMT
  host: fixidu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fixidu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixidu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fixidu
provider_slug: fixidu-com
slug: fixidu-com-domain-security
source_filename: fixidu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixidu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 22:17:39 2026 GMT\n  hsts: false\ndomains:\n- domain: fixidu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fixidu-com/security/fixidu-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Home Services
- On-Demand
- India
- Platform
- Consumer
---
