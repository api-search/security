---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: voyagersearch.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: voyagersearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voyager Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyager Search, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Voyager Search
provider_slug: voyager-search
slug: voyager-search-domain-security
source_filename: voyager-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyagersearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voyagersearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/voyager-search/security/voyager-search-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Geospatial
- Data-Intelligence
- Enterprise
- Search
- Platform
- Company
---
