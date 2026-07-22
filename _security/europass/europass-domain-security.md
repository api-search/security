---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: europasschina.com
  spf: true
hosts:
- cert_expires: Oct 13 05:12:51 2026 GMT
  host: europasschina.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Europass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Europass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Europass
provider_slug: europass
slug: europass-domain-security
source_filename: europass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: europasschina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 05:12:51 2026 GMT\n  hsts: false\ndomains:\n- domain: europasschina.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/europass/refs/heads/main/security/europass-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Digital Agency
- Chinese Tourism
- Mobile Payments
- WeChat
- E-Commerce
- Destination Marketing
- Travel Technology
---
