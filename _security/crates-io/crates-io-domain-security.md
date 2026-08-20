---
api_specs:
- filename: crates-io-config-api-openapi.yml
  format: yaml
  label: crates.io Config API
  slug: crates-io-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-config-api-openapi.yml
- filename: crates-io-crates-api-openapi.yml
  format: yaml
  label: crates.io Crates API
  slug: crates-io-crates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-crates-api-openapi.yml
- filename: crates-io-index-api-openapi.yml
  format: yaml
  label: crates.io Index API
  slug: crates-io-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-index-api-openapi.yml
- filename: crates-io-owners-api-openapi.yml
  format: yaml
  label: crates.io Owners API
  slug: crates-io-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-owners-api-openapi.yml
- filename: crates-io-versions-api-openapi.yml
  format: yaml
  label: crates.io Versions API
  slug: crates-io-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crates.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rust-lang.org
  spf: true
hosts:
- cert_expires: Feb 16 15:26:58 2027 GMT
  host: crates.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: doc.rust-lang.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 14:13:20 2027 GMT
  host: index.crates.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crates Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crates.io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: crates.io
provider_slug: crates-io
slug: crates-io-domain-security
source_filename: crates-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crates.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 15:26:58 2027 GMT\n  hsts: null\n- host: doc.rust-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\n- host: index.crates.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 14:13:20 2027 GMT\n  hsts: false\ndomains:\n- domain: crates.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rust-lang.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/security/crates-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Rust
- Package Registry
- Crates
- Cargo
- Open-Source
- Developer Tools
- Rust Foundation
---
