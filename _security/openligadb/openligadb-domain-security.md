---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openligadb.de
  spf: false
hosts:
- cert_expires: Oct  2 08:26:15 2026 GMT
  host: www.openligadb.de
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openligadb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLigaDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: OpenLigaDB
provider_slug: openligadb
slug: openligadb-domain-security
source_filename: openligadb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openligadb.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:26:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: openligadb.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openligadb/refs/heads/main/security/openligadb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports And Fitness
- Public APIs
---
