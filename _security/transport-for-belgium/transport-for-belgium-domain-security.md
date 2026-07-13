---
description: ''
domains:
- caa:
  - 0 iodef "mailto:bert@irail.be"
  dmarc: false
  dnssec: false
  domain: irail.be
  spf: false
hosts:
- cert_expires: Sep 15 11:23:42 2026 GMT
  host: docs.irail.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Belgium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Belgium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Transport for Belgium
provider_slug: transport-for-belgium
slug: transport-for-belgium-domain-security
source_filename: transport-for-belgium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.irail.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:23:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: irail.be\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:bert@irail.be\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-belgium/refs/heads/main/security/transport-for-belgium-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Transportation
- Public APIs
---
