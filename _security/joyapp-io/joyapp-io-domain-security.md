---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: joyapp.io
  spf: false
hosts:
- cert_expires: Dec  2 16:16:06 2026 GMT
  host: joyapp.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joyapp Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Joy
provider_slug: joyapp-io
slug: joyapp-io-domain-security
source_filename: joyapp-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joyapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 16:16:06 2026 GMT\n  hsts: false\ndomains:\n- domain: joyapp.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/joyapp-io/security/joyapp-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Gaming
- Philippines License
---
