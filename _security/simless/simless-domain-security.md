---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: simless.com
  spf: false
hosts:
- cert_expires: Sep 21 15:32:59 2026 GMT
  host: simless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simless, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Simless
provider_slug: simless
slug: simless-domain-security
source_filename: simless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:32:59 2026 GMT\n  hsts: null\ndomains:\n- domain: simless.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simless/refs/heads/main/security/simless-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
