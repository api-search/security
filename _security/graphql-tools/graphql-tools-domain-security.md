---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: the-guild.dev
  spf: true
hosts:
- cert_expires: Sep 27 10:42:35 2026 GMT
  host: the-guild.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphql Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphQL Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GraphQL Tools
provider_slug: graphql-tools
slug: graphql-tools-domain-security
source_filename: graphql-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-guild.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:42:35 2026 GMT\n  hsts: false\ndomains:\n- domain: the-guild.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphql-tools/refs/heads/main/security/graphql-tools-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- GraphQL
- Schema Stitching
- Schema Merging
- Mocking
- Schema Transformation
- Federation
---
