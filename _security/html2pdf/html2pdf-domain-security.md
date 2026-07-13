---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: html2pdf.app
  spf: true
hosts:
- cert_expires: Sep 29 22:10:06 2026 GMT
  host: html2pdf.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Html2Pdf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Html2PDF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Html2PDF
provider_slug: html2pdf
slug: html2pdf-domain-security
source_filename: html2pdf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: html2pdf.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:10:06 2026 GMT\n  hsts: false\ndomains:\n- domain: html2pdf.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/html2pdf/refs/heads/main/security/html2pdf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Documents And Productivity
- Public APIs
---
