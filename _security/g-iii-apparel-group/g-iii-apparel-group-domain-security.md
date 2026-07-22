---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: g-iii.com
  spf: true
hosts:
- cert_expires: Aug 15 13:29:31 2026 GMT
  host: www.g-iii.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: G Iii Apparel Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G-III Apparel Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: G-III Apparel Group
provider_slug: g-iii-apparel-group
slug: g-iii-apparel-group-domain-security
source_filename: g-iii-apparel-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.g-iii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 13:29:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: g-iii.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g-iii-apparel-group/refs/heads/main/security/g-iii-apparel-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Fashion
- Retail
- Fortune 1000
---
