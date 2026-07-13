---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lordicon.com
  spf: false
hosts:
- cert_expires: Sep 29 10:41:26 2026 GMT
  host: lordicon.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lordicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lordicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lordicon
provider_slug: lordicon
slug: lordicon-domain-security
source_filename: lordicon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lordicon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 10:41:26 2026 GMT\n  hsts: false\ndomains:\n- domain: lordicon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lordicon/refs/heads/main/security/lordicon-domain-security.yml
summary_line: TLSv1.2
tags:
- Art And Design
- Public APIs
---
