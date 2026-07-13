---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: abibliadigital.com.br
  spf: false
hosts:
- cert_expires: Oct  5 23:06:14 2026 GMT
  host: www.abibliadigital.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: A B Blia Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A Bíblia Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: A Bíblia Digital
provider_slug: a-b-blia-digital
slug: a-b-blia-digital-domain-security
source_filename: a-b-blia-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abibliadigital.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:06:14 2026 GMT\n  hsts: false\ndomains:\n- domain: abibliadigital.com.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-b-blia-digital/refs/heads/main/security/a-b-blia-digital-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Books
- Public APIs
---
