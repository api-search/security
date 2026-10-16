---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "zerossl.com"
  - 0 issue "wildcard.pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: clearballot.com
  spf: true
hosts:
- cert_expires: Nov 13 06:08:24 2026 GMT
  host: www.clearballot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearballotgroupinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearballotgroupinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Clearballotgroupinc
provider_slug: clearballotgroupinc
slug: clearballotgroupinc-domain-security
source_filename: clearballotgroupinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearballot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 06:08:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearballot.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"zerossl.com\"\n  - 0 issue \"wildcard.pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearballotgroupinc/refs/heads/main/security/clearballotgroupinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Elections
- Voting
- Security
- Technology
---
