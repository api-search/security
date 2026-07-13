---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kbb.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: developer.kbb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kelley Blue Book Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kelley Blue Book, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kelley Blue Book
provider_slug: kelley-blue-book
slug: kelley-blue-book-domain-security
source_filename: kelley-blue-book-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.kbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kbb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kelley-blue-book/refs/heads/main/security/kelley-blue-book-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vehicle
- Public APIs
---
