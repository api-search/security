---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: joltsynsor.com
  spf: true
hosts:
- cert_expires: Aug 31 01:56:07 2026 GMT
  host: joltsynsor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joltsynsor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joltsynsor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Joltsynsor
provider_slug: joltsynsor
slug: joltsynsor-domain-security
source_filename: joltsynsor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joltsynsor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:56:07 2026 GMT\n  hsts: null\ndomains:\n- domain: joltsynsor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joltsynsor/refs/heads/main/security/joltsynsor-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---
