---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: autoura.com
  spf: true
hosts:
- cert_expires: Oct 17 08:01:02 2026 GMT
  host: www.autoura.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autoura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autoura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Autoura
provider_slug: autoura
slug: autoura-domain-security
source_filename: autoura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autoura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 08:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: autoura.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoura/refs/heads/main/security/autoura-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tourism
- Tours
- Travel
- Destinations
- Experiences
- Digital Tourism
---
