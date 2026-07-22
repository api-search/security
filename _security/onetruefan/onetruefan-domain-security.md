---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onetruefan.com
  spf: false
hosts:
- cert_expires: Sep  8 23:55:43 2026 GMT
  host: onetruefan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onetruefan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneTrueFan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OneTrueFan
provider_slug: onetruefan
slug: onetruefan-domain-security
source_filename: onetruefan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onetruefan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:55:43 2026 GMT\n  hsts: null\ndomains:\n- domain: onetruefan.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetruefan/refs/heads/main/security/onetruefan-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
