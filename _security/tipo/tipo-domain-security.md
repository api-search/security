---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tipo.gov.tw
  spf: true
hosts:
- cert_expires: Sep 10 06:33:34 2026 GMT
  host: tiponet.tipo.gov.tw
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tipo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIPO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TIPO
provider_slug: tipo
slug: tipo-domain-security
source_filename: tipo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tiponet.tipo.gov.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:33:34 2026 GMT\n  hsts: false\ndomains:\n- domain: tipo.gov.tw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tipo/refs/heads/main/security/tipo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Patent
- Public APIs
---
