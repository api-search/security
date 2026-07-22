---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openairpub.com
  spf: false
hosts:
- cert_expires: Oct 17 02:55:11 2026 GMT
  host: openairpub.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openair Publishing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAir Publishing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenAir Publishing
provider_slug: openair-publishing
slug: openair-publishing-domain-security
source_filename: openair-publishing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openairpub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:55:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: openairpub.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openair-publishing/refs/heads/main/security/openair-publishing-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
