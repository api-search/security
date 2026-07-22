---
description: ''
domains:
- caa:
  - 0 issue "zerossl.com"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "wildcard.pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: clearballot.com
  spf: true
hosts:
- cert_expires: Sep 15 02:27:46 2026 GMT
  host: www.clearballot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clear Ballot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Ballot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Clear Ballot
provider_slug: clear-ballot
slug: clear-ballot-domain-security
source_filename: clear-ballot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearballot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:27:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearballot.com\n  dnssec: true\n  caa:\n  - 0 issue \"zerossl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"wildcard.pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-ballot/refs/heads/main/security/clear-ballot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Election Technology
- Voting Systems
- GovTech
- Civic Technology
- Security
---
