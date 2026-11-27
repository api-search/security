---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aitocall.com
  spf: false
hosts:
- cert_expires: Dec  1 05:39:56 2026 GMT
  host: aitocall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aitocall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aitocall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aitocall
provider_slug: aitocall-com
slug: aitocall-com-domain-security
source_filename: aitocall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aitocall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 05:39:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aitocall.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aitocall-com/security/aitocall-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Telephony
- Voice
- Communications
- Korean
---
