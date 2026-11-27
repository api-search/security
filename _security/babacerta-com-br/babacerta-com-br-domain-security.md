---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: babacerta.com.br
  spf: true
hosts:
- cert_expires: Dec 22 19:05:53 2026 GMT
  host: babacerta.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Babá Certa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Babá Certa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Babá Certa
provider_slug: babacerta-com-br
slug: babacerta-com-br-domain-security
source_filename: babacerta-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babacerta.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 19:05:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: babacerta.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/babacerta-com-br/security/babacerta-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Babysitting
- Marketplace
- Verification
- Brazil
- Childcare
---
