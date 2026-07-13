---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wabteccorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wabtec.com
  spf: true
hosts:
- cert_expires: Sep  3 21:02:44 2026 GMT
  host: www.wabteccorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 14:17:28 2026 GMT
  host: one.wabtec.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: pcm.railconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Westinghouse Air Brake Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for westinghouse-air-brake-technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: westinghouse-air-brake-technologies
provider_slug: westinghouse-air-brake-technologies
slug: westinghouse-air-brake-technologies-domain-security
source_filename: westinghouse-air-brake-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wabteccorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 21:02:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: one.wabtec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:17:28 2026 GMT\n  hsts: null\n- host: pcm.railconnect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wabteccorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wabtec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westinghouse-air-brake-technologies/refs/heads/main/security/westinghouse-air-brake-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
---
