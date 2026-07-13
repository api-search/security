---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: savepage.io
  spf: true
hosts:
- cert_expires: Sep 25 04:42:48 2026 GMT
  host: www.savepage.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savepage Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SavePage.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SavePage.io
provider_slug: savepage-io
slug: savepage-io-domain-security
source_filename: savepage-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.savepage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:42:48 2026 GMT\n  hsts: false\ndomains:\n- domain: savepage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savepage-io/refs/heads/main/security/savepage-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
