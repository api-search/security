---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getethos.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.getethos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getethos Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ethos
provider_slug: getethos-com
slug: getethos-com-domain-security
source_filename: getethos-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getethos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getethos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getethos-com/security/getethos-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Insurance
- FinTech
- API
- LifeInsurance
- Digital
---
