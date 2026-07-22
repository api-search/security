---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sabi.com
  spf: true
hosts:
- cert_expires: Sep 13 18:02:41 2026 GMT
  host: sabi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sabi
provider_slug: sabi
slug: sabi-domain-security
source_filename: sabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:02:41 2026 GMT\n  hsts: false\ndomains:\n- domain: sabi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sabi/refs/heads/main/security/sabi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Neural Interface
- Brain-Computer Interface
- Wearable
- Hardware
- Artificial Intelligence
---
