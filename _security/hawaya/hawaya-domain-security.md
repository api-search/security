---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hawaya.com
  spf: true
hosts:
- cert_expires: Oct  4 19:20:44 2026 GMT
  host: www.hawaya.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hawaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hawaya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hawaya
provider_slug: hawaya
slug: hawaya-domain-security
source_filename: hawaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hawaya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:20:44 2026 GMT\n  hsts: false\ndomains:\n- domain: hawaya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawaya/refs/heads/main/security/hawaya-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Dating
- Matchmaking
- Muslim
- Consumer App
- Mobile App
- Match Group
- Discontinued
---
