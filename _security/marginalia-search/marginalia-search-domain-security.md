---
api_specs:
- filename: marginalia-search-openapi.yml
  format: yaml
  label: Marginalia Search API
  slug: marginalia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginalia-search/refs/heads/main/openapi/marginalia-search-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: marginalia-search.com
  spf: true
hosts:
- cert_expires: Sep  1 01:19:04 2026 GMT
  host: marginalia-search.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 01:19:04 2026 GMT
  host: about.marginalia-search.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 01:19:04 2026 GMT
  host: api2.marginalia-search.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marginalia Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marginalia Search, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Marginalia Search
provider_slug: marginalia-search
slug: marginalia-search-domain-security
source_filename: marginalia-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marginalia-search.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:19:04 2026 GMT\n  hsts: null\n- host: about.marginalia-search.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:19:04 2026 GMT\n  hsts: false\n- host: api2.marginalia-search.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:19:04 2026 GMT\n  hsts: null\ndomains:\n- domain: marginalia-search.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marginalia-search/refs/heads/main/security/marginalia-search-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Source
- Search
- Web Search
---
