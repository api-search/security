---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: enlinea.asia
  spf: true
hosts:
- cert_expires: Oct  6 04:37:26 2026 GMT
  host: enlinea.asia
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enlinea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enlinea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enlinea
provider_slug: enlinea
slug: enlinea-domain-security
source_filename: enlinea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enlinea.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:37:26 2026 GMT\n  hsts: null\ndomains:\n- domain: enlinea.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enlinea/refs/heads/main/security/enlinea-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
