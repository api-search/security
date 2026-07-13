---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wns.com
  spf: true
hosts:
- cert_expires: Feb  6 09:22:01 2027 GMT
  host: www.wns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.wns.com
  https: false
- host: api.wns.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wns Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WNS Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WNS Holdings
provider_slug: wns-holdings
slug: wns-holdings-domain-security
source_filename: wns-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 09:22:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wns.com\n  https: false\n- host: api.wns.com\n  https: false\ndomains:\n- domain: wns.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wns-holdings/refs/heads/main/security/wns-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Process Outsourcing
- Analytics
---
