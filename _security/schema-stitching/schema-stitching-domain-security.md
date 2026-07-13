---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: the-guild.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apollographql.com
  spf: true
hosts:
- cert_expires: Sep 27 10:42:35 2026 GMT
  host: the-guild.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 12:55:07 2026 GMT
  host: www.apollographql.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schema Stitching Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schema Stitching, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Schema Stitching
provider_slug: schema-stitching
slug: schema-stitching-domain-security
source_filename: schema-stitching-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-guild.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:42:35 2026 GMT\n  hsts: false\n- host: www.apollographql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 12:55:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: the-guild.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apollographql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schema-stitching/refs/heads/main/security/schema-stitching-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Composition
- API Gateway
- Federation
- GraphQL
- Microservices
- Schema Stitching
- Type Merging
---
