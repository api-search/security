---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imyup.com
  spf: true
hosts:
- cert_expires: Aug 24 23:48:52 2026 GMT
  host: imyup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imyup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imyup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: imyup
provider_slug: imyup
slug: imyup-domain-security
source_filename: imyup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imyup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:48:52 2026 GMT\n  hsts: false\ndomains:\n- domain: imyup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imyup/refs/heads/main/security/imyup-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Content
- Mobile Gaming
- Blog
- Media
- Downloads
---
