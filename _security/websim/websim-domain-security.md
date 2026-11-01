---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: websim.com
  spf: true
hosts:
- cert_expires: Jan  3 12:34:07 2027 GMT
  host: websim.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Websim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Websim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Websim
provider_slug: websim
slug: websim-domain-security
source_filename: websim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: websim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:34:07 2027 GMT\n  hsts: false\ndomains:\n- domain: websim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/websim/security/websim-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
