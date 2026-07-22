---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: withprotege.ai
  spf: true
hosts:
- cert_expires: Sep  6 03:12:55 2026 GMT
  host: www.withprotege.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Protege Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protege, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Protege
provider_slug: protege
slug: protege-domain-security
source_filename: protege-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withprotege.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:12:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: withprotege.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protege/refs/heads/main/security/protege-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Data
- Training Data
- Datasets
- Data Marketplace
- Healthcare
---
