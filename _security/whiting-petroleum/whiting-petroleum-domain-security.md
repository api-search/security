---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chordenergy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: whiting.com
  spf: true
hosts:
- cert_expires: Sep  3 21:48:47 2026 GMT
  host: www.chordenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.whiting.com
  https: false
kind: domain-security
layout: security
method: probed
name: Whiting Petroleum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whiting Petroleum, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Whiting Petroleum
provider_slug: whiting-petroleum
slug: whiting-petroleum-domain-security
source_filename: whiting-petroleum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chordenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 21:48:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.whiting.com\n  https: false\ndomains:\n- domain: chordenergy.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: whiting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiting-petroleum/refs/heads/main/security/whiting-petroleum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Oil And Gas
- Energy
- Upstream
- Williston Basin
- Bakken Shale
- Fortune 1000
---
