---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theaudiodb.com
  spf: false
hosts:
- cert_expires: Aug 24 21:58:01 2026 GMT
  host: www.theaudiodb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theaudiodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheAudioDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TheAudioDB
provider_slug: theaudiodb
slug: theaudiodb-domain-security
source_filename: theaudiodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theaudiodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:58:01 2026 GMT\n  hsts: false\ndomains:\n- domain: theaudiodb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theaudiodb/refs/heads/main/security/theaudiodb-domain-security.yml
summary_line: TLSv1.3
tags:
- Music
- Public APIs
---
