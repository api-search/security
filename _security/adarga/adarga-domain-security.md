---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: adarga.ai
  spf: true
hosts:
- cert_expires: Oct 24 14:03:56 2026 GMT
  host: www.adarga.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adarga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adarga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Adarga
provider_slug: adarga
slug: adarga-domain-security
source_filename: adarga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adarga.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 14:03:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: adarga.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adarga/refs/heads/main/security/adarga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Defense
- National Security
- Intelligence
- Analytics
- Natural Language Processing
- Data Fusion
- Machine Learning
- United Kingdom
---
