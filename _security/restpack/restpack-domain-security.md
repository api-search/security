---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: restpack.io
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: restpack.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Restpack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restpack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Restpack
provider_slug: restpack
slug: restpack-domain-security
source_filename: restpack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restpack.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: restpack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restpack/refs/heads/main/security/restpack-domain-security.yml
summary_line: TLSv1.2
tags:
- Documents And Productivity
- Public APIs
---
