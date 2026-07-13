---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: akitasoftware.com
  spf: false
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
hosts:
- cert_expires: Aug 18 02:52:12 2026 GMT
  host: www.akitasoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akita Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akita Software, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Akita Software
provider_slug: akita-software
slug: akita-software-domain-security
source_filename: akita-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akitasoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:52:12 2026 GMT\n  hsts: null\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akitasoftware.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akita-software/refs/heads/main/security/akita-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acquired
- API Discovery
- API Mapping
- API Observability
- Traffic Analysis
---
