---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: buscazap.com.br
  spf: true
hosts:
- cert_expires: Jan 14 09:40:49 2027 GMT
  host: buscazap.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buscazap Com Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for buscazap-com-br, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: buscazap-com-br
provider_slug: buscazap-com-br
slug: buscazap-com-br-domain-security
source_filename: buscazap-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buscazap.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:40:49 2027 GMT\n  hsts: null\ndomains:\n- domain: buscazap.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buscazap-com-br/security/buscazap-com-br-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
