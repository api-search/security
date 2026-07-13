---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: martinfowler.com
  spf: false
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: jsonapi.org
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: martinfowler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:13:22 2026 GMT
  host: jsonapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 06:09:40 2026 GMT
  host: stateless.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RESTful, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: RESTful
provider_slug: restful
slug: restful-domain-security
source_filename: restful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: martinfowler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jsonapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:13:22 2026 GMT\n  hsts: false\n- host: stateless.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:09:40 2026 GMT\n  hsts: false\ndomains:\n- domain: martinfowler.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: jsonapi.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restful/refs/heads/main/security/restful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- HTTP
- Web Services
---
