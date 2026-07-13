---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:ops@ml.idmgroup.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: collinsdictionary.com
  spf: true
hosts:
- cert_expires: Sep 23 01:21:26 2026 GMT
  host: api.collinsdictionary.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collins, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Collins
provider_slug: collins
slug: collins-domain-security
source_filename: collins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.collinsdictionary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:21:26 2026 GMT\n  hsts: null\ndomains:\n- domain: collinsdictionary.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:ops@ml.idmgroup.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collins/refs/heads/main/security/collins-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dictionaries
- Public APIs
---
