---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weibook.us
  spf: true
hosts:
- cert_expires: Aug 20 19:56:17 2026 GMT
  host: weibook.us
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weibook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeiBook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WeiBook
provider_slug: weibook
slug: weibook-domain-security
source_filename: weibook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weibook.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:56:17 2026 GMT\n  hsts: null\ndomains:\n- domain: weibook.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weibook/refs/heads/main/security/weibook-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
