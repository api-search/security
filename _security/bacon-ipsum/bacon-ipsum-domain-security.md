---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baconipsum.com
  spf: false
hosts:
- cert_expires: Sep 14 16:24:16 2026 GMT
  host: baconipsum.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bacon Ipsum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bacon Ipsum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bacon Ipsum
provider_slug: bacon-ipsum
slug: bacon-ipsum-domain-security
source_filename: bacon-ipsum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baconipsum.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 16:24:16 2026 GMT\n  hsts: false\ndomains:\n- domain: baconipsum.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bacon-ipsum/refs/heads/main/security/bacon-ipsum-domain-security.yml
summary_line: TLSv1.2
tags:
- Test Data
- Public APIs
---
