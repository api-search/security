---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rootr.io
  spf: true
hosts:
- cert_expires: Dec  3 06:34:40 2026 GMT
  host: rootr.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rootr Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rootr-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: rootr-io
provider_slug: rootr-io
slug: rootr-io-domain-security
source_filename: rootr-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rootr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 06:34:40 2026 GMT\n  hsts: false\ndomains:\n- domain: rootr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rootr-io/security/rootr-io-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- RAG
- Collaboration
- Documentation
- MCP
- TeamKnowledge
---
