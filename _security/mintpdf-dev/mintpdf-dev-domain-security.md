---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mintpdf.dev
  spf: true
hosts:
- cert_expires: Jan  8 18:48:24 2027 GMT
  host: mintpdf.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mintpdf Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mintpdf-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mintpdf-dev
provider_slug: mintpdf-dev
slug: mintpdf-dev-domain-security
source_filename: mintpdf-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mintpdf.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:48:24 2027 GMT\n  hsts: false\ndomains:\n- domain: mintpdf.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mintpdf-dev/security/mintpdf-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- PDF
- Markdown
- HTML
---
