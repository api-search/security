---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ratter.com
  spf: false
hosts:
- cert_expires: Oct 15 11:39:18 2026 GMT
  host: ratter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ratter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ratter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ratter
provider_slug: ratter
slug: ratter-domain-security
source_filename: ratter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ratter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:39:18 2026 GMT\n  hsts: false\ndomains:\n- domain: ratter.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ratter/refs/heads/main/security/ratter-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
