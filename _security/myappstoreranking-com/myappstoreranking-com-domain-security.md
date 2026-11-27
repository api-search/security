---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myappstoreranking.com
  spf: true
hosts:
- cert_expires: Feb  9 16:07:51 2027 GMT
  host: myappstoreranking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: My App Store Ranking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for My App Store Ranking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: My App Store Ranking
provider_slug: myappstoreranking-com
slug: myappstoreranking-com-domain-security
source_filename: myappstoreranking-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myappstoreranking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 16:07:51 2027 GMT\n  hsts: false\ndomains:\n- domain: myappstoreranking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/myappstoreranking-com/security/myappstoreranking-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AppRanking
- Mobile Analytics
- Competitor Intelligence
- Artificial Intelligence
- Software-as-a-Service
---
