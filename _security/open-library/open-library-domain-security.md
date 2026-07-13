---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openlibrary.org
  spf: false
hosts:
- cert_expires: Sep 28 23:05:19 2026 GMT
  host: openlibrary.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:08:21 2026 GMT
  host: covers.openlibrary.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Library Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Library, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Library
provider_slug: open-library
slug: open-library-domain-security
source_filename: open-library-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openlibrary.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:05:19 2026 GMT\n  hsts: false\n- host: covers.openlibrary.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:08:21 2026 GMT\n  hsts: false\ndomains:\n- domain: openlibrary.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-library/refs/heads/main/security/open-library-domain-security.yml
summary_line: TLSv1.3
tags:
- Authors
- Books
- Catalog
- Covers
- Libraries
- Open Data
- Reading Lists
- Search
- Subjects
---
