---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jamendo.com
  spf: true
hosts:
- cert_expires: Aug 30 23:20:47 2026 GMT
  host: developer.jamendo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jamendo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jamendo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jamendo
provider_slug: jamendo
slug: jamendo-domain-security
source_filename: jamendo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.jamendo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:20:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jamendo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jamendo/refs/heads/main/security/jamendo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Music
- Public APIs
---
