---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usebounce.com
  spf: true
hosts:
- cert_expires: Jan 21 15:57:54 2027 GMT
  host: usebounce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usebounce Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bounce
provider_slug: usebounce-com
slug: usebounce-com-domain-security
source_filename: usebounce-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usebounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 15:57:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usebounce.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/usebounce-com/security/usebounce-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Luggage Storage
- Travel
- Local Partnerships
---
