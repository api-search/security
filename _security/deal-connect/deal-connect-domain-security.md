---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deal-connect.co.jp
  spf: true
hosts:
- cert_expires: Sep 26 00:01:02 2026 GMT
  host: deal-connect.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deal Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deal Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deal Connect
provider_slug: deal-connect
slug: deal-connect-domain-security
source_filename: deal-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deal-connect.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:01:02 2026 GMT\n  hsts: false\ndomains:\n- domain: deal-connect.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deal-connect/refs/heads/main/security/deal-connect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
