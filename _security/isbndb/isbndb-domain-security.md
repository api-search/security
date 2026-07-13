---
api_specs:
- filename: doc.json
  format: json
  label: ISBNdb API
  slug: isbndb-api
  spec_type: OpenAPI
  url: https://api2.isbndb.com/doc.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: isbndb.com
  spf: true
hosts:
- cert_expires: Sep 22 11:25:29 2026 GMT
  host: isbndb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:13:13 2026 GMT
  host: api2.isbndb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Isbndb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISBNdb, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ISBNdb
provider_slug: isbndb
slug: isbndb-domain-security
source_filename: isbndb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isbndb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:25:29 2026 GMT\n  hsts: false\n- host: api2.isbndb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:13:13 2026 GMT\n  hsts: null\ndomains:\n- domain: isbndb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/security/isbndb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Books
- ISBN
- Publishing
- Metadata
- Library
- Bibliography
---
