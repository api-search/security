---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bandsaas.com
  spf: true
hosts:
- cert_expires: Dec  4 10:21:07 2026 GMT
  host: bandsaas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BandSaaS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BandSaaS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BandSaaS
provider_slug: bandsaas-com
slug: bandsaas-com-domain-security
source_filename: bandsaas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bandsaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 10:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bandsaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bandsaas-com/security/bandsaas-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Music
- Licensing
- Artists
- Platform
---
