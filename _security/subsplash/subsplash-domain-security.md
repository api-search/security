---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:ops+security@subsplash.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: subsplash.com
  spf: true
hosts:
- cert_expires: Aug 16 09:42:59 2026 GMT
  host: www.subsplash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: developer.subsplash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: core.subsplash.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Subsplash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subsplash, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Subsplash
provider_slug: subsplash
slug: subsplash-domain-security
source_filename: subsplash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subsplash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.subsplash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: core.subsplash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: subsplash.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:ops+security@subsplash.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subsplash/refs/heads/main/security/subsplash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Church
- Ministry
- Nonprofit
- Giving
- Media
- Church Management
- ChMS
- Mobile Apps
- Partner API
---
