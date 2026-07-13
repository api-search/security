---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iata.org
  spf: true
hosts:
- cert_expires: Sep 27 14:07:57 2026 GMT
  host: developer.iata.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:08:46 2026 GMT
  host: www.iata.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: api.developer.iata.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Iata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IATA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IATA
provider_slug: iata
slug: iata-domain-security
source_filename: iata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.iata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.iata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.developer.iata.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: iata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iata/refs/heads/main/security/iata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Airports
- Aviation
- Cargo
- Standards
- Travel
---
