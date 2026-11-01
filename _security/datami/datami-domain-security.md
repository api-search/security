---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: internetpatrocinada.com.br
  spf: true
hosts:
- cert_expires: Dec 15 02:18:45 2026 GMT
  host: internetpatrocinada.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datami
provider_slug: datami
slug: datami-domain-security
source_filename: datami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internetpatrocinada.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:18:45 2026 GMT\n  hsts: false\ndomains:\n- domain: internetpatrocinada.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datami/security/datami-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telecommunications
- Data Sponsorship
- Digital Inclusion
- Public Services
---
