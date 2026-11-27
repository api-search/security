---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: newread.com.br
  spf: true
hosts:
- cert_expires: Jan 24 11:16:35 2027 GMT
  host: newread.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NewRead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewRead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NewRead
provider_slug: newread-com-br
slug: newread-com-br-domain-security
source_filename: newread-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newread.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 11:16:35 2027 GMT\n  hsts: false\ndomains:\n- domain: newread.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/newread-com-br/security/newread-com-br-domain-security.yml
summary_line: TLSv1.3
tags:
- Water
- Gas
- Condominium
- Billing
- Brazil
---
