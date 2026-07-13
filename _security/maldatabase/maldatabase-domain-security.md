---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: maldatabase.com
  spf: true
hosts:
- cert_expires: Oct  9 12:12:40 2026 GMT
  host: maldatabase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maldatabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MalDatabase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MalDatabase
provider_slug: maldatabase
slug: maldatabase-domain-security
source_filename: maldatabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maldatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:12:40 2026 GMT\n  hsts: false\ndomains:\n- domain: maldatabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maldatabase/refs/heads/main/security/maldatabase-domain-security.yml
summary_line: TLSv1.3
tags:
- Anti Malware
- Public APIs
---
