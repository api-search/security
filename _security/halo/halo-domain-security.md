---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: haloapi.com
  spf: false
hosts:
- cert_expires: Dec 29 01:17:00 2026 GMT
  host: developer.haloapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Halo
provider_slug: halo
slug: halo-domain-security
source_filename: halo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.haloapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 01:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: haloapi.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo/refs/heads/main/security/halo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
