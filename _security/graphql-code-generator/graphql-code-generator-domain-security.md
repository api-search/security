---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
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
name: Graphql Code Generator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphQL Code Generator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GraphQL Code Generator
provider_slug: graphql-code-generator
slug: graphql-code-generator-domain-security
source_filename: graphql-code-generator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-guild.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:42:35 2026 GMT\n  hsts: false\ndomains:\n- domain: the-guild.dev\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphql-code-generator/refs/heads/main/security/graphql-code-generator-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- GraphQL
- Code Generation
- TypeScript
- Developer Tools
- Open Source
---
