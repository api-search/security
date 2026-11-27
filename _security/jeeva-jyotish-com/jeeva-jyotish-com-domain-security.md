---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jeeva-jyotish.com
  spf: true
hosts:
- cert_expires: Feb  4 01:07:32 2027 GMT
  host: jeeva-jyotish.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jyotish Life Mapper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jyotish Life Mapper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jyotish Life Mapper
provider_slug: jeeva-jyotish-com
slug: jeeva-jyotish-com-domain-security
source_filename: jeeva-jyotish-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeeva-jyotish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 01:07:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jeeva-jyotish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jeeva-jyotish-com/security/jeeva-jyotish-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Astrology
- Vedic
- LifeMapping
- Charting
- Open Source
---
