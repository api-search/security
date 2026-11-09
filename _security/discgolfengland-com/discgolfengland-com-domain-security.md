---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: discgolfengland.com
  spf: true
hosts:
- cert_expires: Dec 19 01:31:18 2026 GMT
  host: discgolfengland.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Discgolfengland Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for English Disc Golf Association, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: English Disc Golf Association
provider_slug: discgolfengland-com
slug: discgolfengland-com-domain-security
source_filename: discgolfengland-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: discgolfengland.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:31:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: discgolfengland.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/discgolfengland-com/security/discgolfengland-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Disc Golf
- Sports
- United Kingdom
- Non-Profit
- Community
---
