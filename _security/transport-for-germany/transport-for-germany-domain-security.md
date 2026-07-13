---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deutschebahn.com
  spf: true
hosts:
- cert_expires: Oct  4 03:09:50 2026 GMT
  host: data.deutschebahn.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Germany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Germany, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport for Germany
provider_slug: transport-for-germany
slug: transport-for-germany-domain-security
source_filename: transport-for-germany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.deutschebahn.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 03:09:50 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: deutschebahn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-germany/refs/heads/main/security/transport-for-germany-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
