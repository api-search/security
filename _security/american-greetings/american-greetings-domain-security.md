---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: americangreetings.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.americangreetings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.americangreetings.com
  https: false
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.americangreetings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Greetings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Greetings, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Greetings
provider_slug: american-greetings
slug: american-greetings-domain-security
source_filename: american-greetings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.americangreetings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\n- host: developer.americangreetings.com\n  https: false\n- host: api.americangreetings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: americangreetings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-greetings/refs/heads/main/security/american-greetings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Greeting Cards
- Gift Wrap
- Celebration
---
