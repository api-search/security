---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: python.org
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Feb 14 13:03:45 2027 GMT
  host: www.python.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 13:03:45 2027 GMT
  host: docs.python.org
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: requests.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Python Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Python Standard Library and Popular, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Python Standard Library and Popular
provider_slug: python
slug: python-domain-security
source_filename: python-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.python.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 13:03:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.python.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 13:03:45 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: requests.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: python.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  spf: false\n  dmarc:\
  \ false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/python/refs/heads/main/security/python-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Frameworks
- Libraries
- Programming Language
- Python
---
