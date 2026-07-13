---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:informationsecurityalerts@psc.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pipersandler.com
  spf: false
hosts:
- cert_expires: Feb 10 21:13:59 2027 GMT
  host: www.pipersandler.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- host: developer.pipersandler.com
  https: false
- host: api.pipersandler.com
  https: false
kind: domain-security
layout: security
method: probed
name: Piper Sandler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piper Sandler Companies, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Piper Sandler Companies
provider_slug: piper-sandler
slug: piper-sandler-domain-security
source_filename: piper-sandler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pipersandler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 21:13:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.pipersandler.com\n  https: false\n- host: api.pipersandler.com\n  https: false\ndomains:\n- domain: pipersandler.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:informationsecurityalerts@psc.com\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piper-sandler/refs/heads/main/security/piper-sandler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Investment Banking
- Institutional Brokerage
---
