---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: squiggle.com.au
  spf: false
hosts:
- cert_expires: Sep  6 17:03:32 2026 GMT
  host: api.squiggle.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squiggle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squiggle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Squiggle
provider_slug: squiggle
slug: squiggle-domain-security
source_filename: squiggle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.squiggle.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:03:32 2026 GMT\n  hsts: false\ndomains:\n- domain: squiggle.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squiggle/refs/heads/main/security/squiggle-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
