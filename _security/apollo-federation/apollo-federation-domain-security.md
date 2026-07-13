---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apollographql.com
  spf: true
hosts:
- cert_expires: Aug 13 12:55:07 2026 GMT
  host: www.apollographql.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Federation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo Federation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apollo Federation
provider_slug: apollo-federation
slug: apollo-federation-domain-security
source_filename: apollo-federation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apollographql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 12:55:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apollographql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-federation/refs/heads/main/security/apollo-federation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- Federation
- GraphQL
- Microservices
- Open Source
- Subgraphs
- Supergraph
---
