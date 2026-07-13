---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: idexx.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vetconnectplus.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.idexx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 20:20:56 2026 GMT
  host: developer.vetconnectplus.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Idexx Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IDEXX, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: IDEXX
provider_slug: idexx-labs
slug: idexx-labs-domain-security
source_filename: idexx-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.idexx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vetconnectplus.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 20:20:56 2026 GMT\n  hsts: false\ndomains:\n- domain: idexx.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: vetconnectplus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idexx-labs/refs/heads/main/security/idexx-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Veterinary
- Diagnostics
- Reference Labs
- Diagnostic Imaging
- Animal Health
- Healthcare
- VetConnect PLUS
- Web PACS
- Partner Gated
---
