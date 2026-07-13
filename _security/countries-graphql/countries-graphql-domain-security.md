---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trevorblades.com
  spf: false
hosts:
- cert_expires: Sep 30 03:12:41 2026 GMT
  host: countries.trevorblades.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Countries Graphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Countries GraphQL API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Countries GraphQL API
provider_slug: countries-graphql
slug: countries-graphql-domain-security
source_filename: countries-graphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: countries.trevorblades.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:12:41 2026 GMT\n  hsts: null\ndomains:\n- domain: trevorblades.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countries-graphql/refs/heads/main/security/countries-graphql-domain-security.yml
summary_line: TLSv1.3
tags:
- GraphQL
- Countries
- Geography
- Open Data
- Free
- Languages
- Continents
---
