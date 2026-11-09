---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dbplanner.io
  spf: true
hosts:
- cert_expires: Dec 18 10:46:38 2026 GMT
  host: dbplanner.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dbplanner Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DB Planner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DB Planner
provider_slug: dbplanner-io
slug: dbplanner-io-domain-security
source_filename: dbplanner-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dbplanner.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 10:46:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: dbplanner.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dbplanner-io/security/dbplanner-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database Diagram
- ER Diagram
- DBML
- Real-Time Collaboration
- SQL Import
- Code Export
- AI Design
---
