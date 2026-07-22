---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geneva.com
  spf: true
hosts:
- cert_expires: Sep 10 11:19:44 2026 GMT
  host: geneva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geneva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geneva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Geneva
provider_slug: geneva
slug: geneva-domain-security
source_filename: geneva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geneva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:19:44 2026 GMT\n  hsts: false\ndomains:\n- domain: geneva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geneva/refs/heads/main/security/geneva-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social
- Community
- Group Chat
- Messaging
- Communities
- Consumer App
- Crypto Web3
---
