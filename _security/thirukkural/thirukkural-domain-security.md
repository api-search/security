---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: web.app
  spf: false
hosts:
- cert_expires: Aug 18 17:14:16 2026 GMT
  host: api-thirukkural.web.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thirukkural Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thirukkural, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Thirukkural
provider_slug: thirukkural
slug: thirukkural-domain-security
source_filename: thirukkural-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-thirukkural.web.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:14:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: web.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirukkural/refs/heads/main/security/thirukkural-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Books
- Public APIs
---
