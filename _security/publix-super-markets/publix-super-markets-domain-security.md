---
description: ''
domains:
- caa:
  - 0 issuewild "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:DataProtectionTeam@publix.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: publix.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.publix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Publix Super Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publix Super Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Publix Super Markets
provider_slug: publix-super-markets
slug: publix-super-markets-domain-security
source_filename: publix-super-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.publix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: publix.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:DataProtectionTeam@publix.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publix-super-markets/refs/heads/main/security/publix-super-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Grocery
- Supermarket
- Retail
- Pharmacy
---
