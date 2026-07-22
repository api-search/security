---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tweezr.io
  spf: true
hosts:
- cert_expires: Sep 27 12:14:49 2026 GMT
  host: tweezr.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tweezr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tweezr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tweezr
provider_slug: tweezr
slug: tweezr-domain-security
source_filename: tweezr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tweezr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:14:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tweezr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweezr/refs/heads/main/security/tweezr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legacy Modernization
- Mainframe
- Banking
- Financial Services
- System Intelligence
- Artificial Intelligence
---
