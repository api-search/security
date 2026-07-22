---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gqlstandards.org
  spf: false
hosts:
- cert_expires: Sep 25 08:52:15 2026 GMT
  host: www.gqlstandards.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graph Query Language Gql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graph Query Language (GQL), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Graph Query Language (GQL)
provider_slug: graph-query-language-gql
slug: graph-query-language-gql-domain-security
source_filename: graph-query-language-gql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gqlstandards.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:52:15 2026 GMT\n  hsts: false\ndomains:\n- domain: gqlstandards.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graph-query-language-gql/refs/heads/main/security/graph-query-language-gql-domain-security.yml
summary_line: TLSv1.3
tags:
- Database
- Graph Database
- ISO Standard
- Query Language
- Standard
- Property Graph
---
