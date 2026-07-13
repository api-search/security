---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chaoss.community
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Oct  4 15:50:42 2026 GMT
  host: chaoss.community
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: oss-augur.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ai.chaoss.io
  https: false
kind: domain-security
layout: security
method: probed
name: Chaoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAOSS, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CHAOSS
provider_slug: chaoss
slug: chaoss-domain-security
source_filename: chaoss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaoss.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:50:42 2026 GMT\n  hsts: false\n- host: oss-augur.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ai.chaoss.io\n  https: false\ndomains:\n- domain: chaoss.community\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/security/chaoss-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Analytics
- Community Health
- DEI
- Linux Foundation
- Metrics
- Observability
- Open Source
- Risk
- Sustainability
---
