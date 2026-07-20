---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: falconx.io
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Oct  1 08:31:02 2026 GMT
  host: www.falconx.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:37:38 2026 GMT
  host: falconx.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 01:31:54 2026 GMT
  host: api.falconx.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Falconx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FalconX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FalconX
provider_slug: falconx
slug: falconx-domain-security
source_filename: falconx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.falconx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:31:02 2026 GMT\n  hsts: false\n- host: falconx.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.falconx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: falconx.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/falconx/refs/heads/main/security/falconx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Prime Brokerage
- Trading
- Institutional
- Financial Services
- Custody
- Derivatives
- OTC
---
