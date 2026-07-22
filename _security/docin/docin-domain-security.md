---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docin.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: docin.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Docin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for docin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: docin
provider_slug: docin
slug: docin-domain-security
source_filename: docin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: docin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docin/refs/heads/main/security/docin-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Documents
- Document Sharing
- Content
- Publishing
- Education
- China
---
