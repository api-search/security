---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: khronos.org
  spf: true
hosts:
- cert_expires: Nov 29 23:31:38 2026 GMT
  host: www.khronos.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Khronos Group Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Khronos Group, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Khronos Group, Inc.
provider_slug: the-khronos-group-inc
slug: the-khronos-group-inc-domain-security
source_filename: the-khronos-group-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.khronos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: khronos.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/the-khronos-group-inc/security/the-khronos-group-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open-Standards
- Graphics
- AR/VR
- Compute
- Consortium
---
