---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mkdocs.org
  spf: false
hosts:
- cert_expires: Sep 23 18:45:51 2026 GMT
  host: www.mkdocs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mkdocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MkDocs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MkDocs
provider_slug: mkdocs
slug: mkdocs-domain-security
source_filename: mkdocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mkdocs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:45:51 2026 GMT\n  hsts: false\ndomains:\n- domain: mkdocs.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mkdocs/refs/heads/main/security/mkdocs-domain-security.yml
summary_line: TLSv1.3
tags:
- Documentation
- Markdown
- Open Source
- Python
- Static Site Generator
---
