---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ford.com
  spf: true
hosts:
- host: developer.ford.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Sep 21 10:48:50 2026 GMT
  host: www.ford.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 06:24:55 2026 GMT
  host: api.mps.ford.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ford Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ford, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ford
provider_slug: ford
slug: ford-domain-security
source_filename: ford-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ford.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.ford.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:48:50 2026 GMT\n  hsts: null\n- host: api.mps.ford.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:24:55 2026 GMT\n  hsts: null\ndomains:\n- domain: ford.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/security/ford-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automobiles
- Cars
- Vehicles
---
