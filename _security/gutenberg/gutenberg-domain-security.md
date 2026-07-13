---
api_specs:
- filename: books
  format: yaml
  label: Gutendex API
  slug: gutendex
  spec_type: OpenAPI
  url: https://gutendex.com/books
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gutenberg.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: gutendex.com
  spf: false
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.gutenberg.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 10:44:01 2026 GMT
  host: gutendex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gutenberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Project Gutenberg, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Project Gutenberg
provider_slug: gutenberg
slug: gutenberg-domain-security
source_filename: gutenberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gutenberg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: gutendex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 10:44:01 2026 GMT\n  hsts: false\ndomains:\n- domain: gutenberg.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: gutendex.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gutenberg/refs/heads/main/security/gutenberg-domain-security.yml
summary_line: TLSv1.3
tags:
- Books
- Ebooks
- Public Domain
- Literature
- Library
- Metadata
- EPUB
---
