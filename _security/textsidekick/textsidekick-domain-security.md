---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: textsidekick.com
  spf: true
hosts:
- cert_expires: Sep 28 06:15:53 2026 GMT
  host: textsidekick.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textsidekick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Textsidekick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Textsidekick
provider_slug: textsidekick
slug: textsidekick-domain-security
source_filename: textsidekick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textsidekick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: textsidekick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textsidekick/refs/heads/main/security/textsidekick-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- SMS
- Frontline Workers
- Workforce Communication
- Knowledge Management
- Work Orders
- Artificial Intelligence
- Y Combinator
---
