---
api_specs:
- filename: gutendex-api-openapi.yml
  format: yaml
  label: Gutendex Books API
  slug: books
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gutendex/refs/heads/main/openapi/gutendex-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gutendex.com
  spf: false
hosts:
- cert_expires: Sep 12 10:44:01 2026 GMT
  host: gutendex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gutendex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gutendex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gutendex
provider_slug: gutendex
slug: gutendex-domain-security
source_filename: gutendex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gutendex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 10:44:01 2026 GMT\n  hsts: false\ndomains:\n- domain: gutendex.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gutendex/refs/heads/main/security/gutendex-domain-security.yml
summary_line: TLSv1.3
tags:
- Books
- Catalog
- Ebooks
- Library
- Literature
- Metadata
- Open Source
- Project Gutenberg
- Public APIs
- Public Domain
---
