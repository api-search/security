---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencypher.org
  spf: false
hosts:
- cert_expires: Sep 18 21:56:21 2026 GMT
  host: opencypher.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencypher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openCypher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: openCypher
provider_slug: opencypher
slug: opencypher-domain-security
source_filename: opencypher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencypher.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:56:21 2026 GMT\n  hsts: false\ndomains:\n- domain: opencypher.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencypher/refs/heads/main/security/opencypher-domain-security.yml
summary_line: TLSv1.3
tags:
- Graph Database
- Neo4j
- openCypher
- Query Language
---
