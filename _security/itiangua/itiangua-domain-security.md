---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: itiangua.com
  spf: false
hosts:
- cert_expires: Sep 17 05:09:29 2026 GMT
  host: itiangua.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itiangua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for itiangua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: itiangua
provider_slug: itiangua
slug: itiangua-domain-security
source_filename: itiangua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itiangua.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:09:29 2026 GMT\n  hsts: null\ndomains:\n- domain: itiangua.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itiangua/refs/heads/main/security/itiangua-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
