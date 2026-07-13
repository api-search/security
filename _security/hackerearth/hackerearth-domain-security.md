---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:support@hackerearth.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hackerearth.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: www.hackerearth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hackerearth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hackerearth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hackerearth
provider_slug: hackerearth
slug: hackerearth-domain-security
source_filename: hackerearth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hackerearth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hackerearth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:support@hackerearth.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackerearth/refs/heads/main/security/hackerearth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Programming
- Public APIs
---
