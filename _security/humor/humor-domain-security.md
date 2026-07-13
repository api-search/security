---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humorapi.com
  spf: false
hosts:
- cert_expires: Sep 14 15:56:50 2026 GMT
  host: humorapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Humor
provider_slug: humor
slug: humor-domain-security
source_filename: humor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humorapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:56:50 2026 GMT\n  hsts: false\ndomains:\n- domain: humorapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humor/refs/heads/main/security/humor-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
