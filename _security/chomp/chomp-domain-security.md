---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chompthis.com
  spf: true
hosts:
- cert_expires: Sep 28 06:05:14 2026 GMT
  host: chompthis.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chomp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chomp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chomp
provider_slug: chomp
slug: chomp-domain-security
source_filename: chomp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chompthis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 06:05:14 2026 GMT\n  hsts: false\ndomains:\n- domain: chompthis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chomp/refs/heads/main/security/chomp-domain-security.yml
summary_line: TLSv1.2
tags:
- Food And Drink
- Public APIs
---
