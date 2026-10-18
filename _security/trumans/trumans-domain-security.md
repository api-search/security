---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trumans.com
  spf: false
hosts:
- cert_expires: Jan 19 01:41:21 2027 GMT
  host: trumans.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trumans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truman''s, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Truman's
provider_slug: trumans
slug: trumans-domain-security
source_filename: trumans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trumans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 01:41:21 2027 GMT\n  hsts: null\ndomains:\n- domain: trumans.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trumans/refs/heads/main/security/trumans-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Venture
- Portfolio
- Startups
- Technology
---
