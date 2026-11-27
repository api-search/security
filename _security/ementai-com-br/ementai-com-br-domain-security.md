---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ementai.com.br
  spf: true
hosts:
- cert_expires: Jan 14 05:12:49 2027 GMT
  host: ementai.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EmentAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmentAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EmentAI
provider_slug: ementai-com-br
slug: ementai-com-br-domain-security
source_filename: ementai-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ementai.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 05:12:49 2027 GMT\n  hsts: false\ndomains:\n- domain: ementai.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ementai-com-br/security/ementai-com-br-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Legal Tech
- Brazil
- JudicialData
- OpenAI
---
