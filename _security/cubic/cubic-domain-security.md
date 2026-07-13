---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cubic.com
  spf: true
hosts:
- cert_expires: Sep 23 07:06:13 2026 GMT
  host: www.cubic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:06:13 2026 GMT
  host: developer.cubic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.cubic.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cubic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubic Corporation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cubic Corporation
provider_slug: cubic
slug: cubic-domain-security
source_filename: cubic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:06:13 2026 GMT\n  hsts: false\n- host: developer.cubic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:06:13 2026 GMT\n  hsts: false\n- host: api.cubic.com\n  https: false\ndomains:\n- domain: cubic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubic/refs/heads/main/security/cubic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Transportation
- Technology
---
