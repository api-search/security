---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lifemote.com
  spf: false
hosts:
- cert_expires: Sep 22 18:02:00 2026 GMT
  host: lifemote.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lifemote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lifemote, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lifemote
provider_slug: lifemote
slug: lifemote-domain-security
source_filename: lifemote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifemote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lifemote.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifemote/refs/heads/main/security/lifemote-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Networking
- Wi-Fi
- Broadband
- Telecommunications
- Analytics
- Artificial Intelligence
- Customer Experience
- Network Observability
- Internet Service Providers
---
