---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: triliumnotes.org
  spf: false
hosts:
- cert_expires: Dec 16 02:08:59 2026 GMT
  host: triliumnotes.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Triliumnotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trilium Notes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trilium Notes
provider_slug: triliumnotes
slug: triliumnotes-domain-security
source_filename: triliumnotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triliumnotes.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 02:08:59 2026 GMT\n  hsts: false\ndomains:\n- domain: triliumnotes.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/triliumnotes/security/triliumnotes-domain-security.yml
summary_line: TLSv1.3
tags:
- Note-taking
- Open-source
- Knowledge-base
- Hierarchical
- REST API
---
