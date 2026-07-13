---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dgraph.io
  spf: true
hosts:
- host: site.dgraph.io
  https: false
- cert_expires: Aug 27 03:38:31 2026 GMT
  host: docs.dgraph.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: cloud.dgraph.io
  https: false
kind: domain-security
layout: security
method: probed
name: Dgraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dgraph, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dgraph
provider_slug: dgraph
slug: dgraph-domain-security
source_filename: dgraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: site.dgraph.io\n  https: false\n- host: docs.dgraph.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 03:38:31 2026 GMT\n  hsts: false\n- host: cloud.dgraph.io\n  https: false\ndomains:\n- domain: dgraph.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dgraph/refs/heads/main/security/dgraph-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- GraphQL
- Graph Database
- Distributed Database
- Real-Time
- Open Source
- Knowledge Graph
---
