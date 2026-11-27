---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easypdf.fr
  spf: true
hosts:
- cert_expires: Dec 31 01:25:14 2026 GMT
  host: easypdf.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EasyPDF Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyPDF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EasyPDF
provider_slug: easypdf-fr
slug: easypdf-fr-domain-security
source_filename: easypdf-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easypdf.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 01:25:14 2026 GMT\n  hsts: false\ndomains:\n- domain: easypdf.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easypdf-fr/security/easypdf-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PDF
- Artificial Intelligence
- Editor
- Software-as-a-Service
- Free
---
