---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tapuzinski.com
  spf: false
hosts:
- cert_expires: Feb 11 12:45:05 2027 GMT
  host: tapuzinski.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tapuzinski Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tapuzinski Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Tapuzinski Market
provider_slug: tapuzinski-com
slug: tapuzinski-com-domain-security
source_filename: tapuzinski-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tapuzinski.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 12:45:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tapuzinski.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tapuzinski-com/security/tapuzinski-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
