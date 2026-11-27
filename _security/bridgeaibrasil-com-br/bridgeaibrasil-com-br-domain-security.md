---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bridgeaibrasil.com.br
  spf: false
hosts:
- cert_expires: Jan 28 21:45:13 2027 GMT
  host: bridgeaibrasil.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: bridgeaibrasil-com-br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bridgeaibrasil-com-br, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: bridgeaibrasil-com-br
provider_slug: bridgeaibrasil-com-br
slug: bridgeaibrasil-com-br-domain-security
source_filename: bridgeaibrasil-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgeaibrasil.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 21:45:13 2027 GMT\n  hsts: false\ndomains:\n- domain: bridgeaibrasil.com.br\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bridgeaibrasil-com-br/security/bridgeaibrasil-com-br-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
