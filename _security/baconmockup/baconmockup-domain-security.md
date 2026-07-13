---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baconmockup.com
  spf: false
hosts:
- cert_expires: Aug 22 18:38:28 2026 GMT
  host: baconmockup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Baconmockup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BaconMockup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BaconMockup
provider_slug: baconmockup
slug: baconmockup-domain-security
source_filename: baconmockup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baconmockup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 18:38:28 2026 GMT\n  hsts: false\ndomains:\n- domain: baconmockup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baconmockup/refs/heads/main/security/baconmockup-domain-security.yml
summary_line: TLSv1.2
tags:
- Food And Drink
- Public APIs
---
