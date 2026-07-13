---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docusaurus.io
  spf: true
hosts:
- cert_expires: Oct  4 20:55:46 2026 GMT
  host: docusaurus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docusaurus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docusaurus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Docusaurus
provider_slug: docusaurus
slug: docusaurus-domain-security
source_filename: docusaurus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docusaurus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:55:46 2026 GMT\n  hsts: false\ndomains:\n- domain: docusaurus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docusaurus/refs/heads/main/security/docusaurus-domain-security.yml
summary_line: TLSv1.3
tags:
- Documentation
- Open Source
- React
- Static Site Generator
- Developer Portals
---
