---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: riverlane.com
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
- cert_expires: Oct 17 06:42:48 2026 GMT
  host: www.riverlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:31:53 2026 GMT
  host: deltakit.readthedocs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 05:45:42 2026 GMT
  host: deltakit.riverlane.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riverlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riverlane, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Riverlane
provider_slug: riverlane
slug: riverlane-domain-security
source_filename: riverlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riverlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: deltakit.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:31:53 2026 GMT\n  hsts: false\n- host: deltakit.riverlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 05:45:42 2026 GMT\n  hsts: false\ndomains:\n- domain: riverlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riverlane/refs/heads/main/security/riverlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- quantum-computing
- quantum-error-correction
- decoders
- scientific-computing
- python-sdk
- graphql
- simulation
- research-tools
- open-source
- hpc
---
