---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metagenomi.co
  spf: true
hosts:
- cert_expires: Oct 23 22:05:16 2026 GMT
  host: metagenomi.co
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metagenomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metagenomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metagenomi
provider_slug: metagenomi
slug: metagenomi-domain-security
source_filename: metagenomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metagenomi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 22:05:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: metagenomi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metagenomi/refs/heads/main/security/metagenomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Gene Editing
- CRISPR
- Genetic Medicine
- Genomics
- Drug Discovery
- Life Sciences
- Machine-Learning
- Metagenomics
- Research
---
