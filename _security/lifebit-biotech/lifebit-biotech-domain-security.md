---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lifebit.ai
  spf: true
hosts:
- cert_expires: Aug 31 18:05:21 2026 GMT
  host: lifebit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: cloudos.lifebit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lifebit Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lifebit Biotech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lifebit Biotech
provider_slug: lifebit-biotech
slug: lifebit-biotech-domain-security
source_filename: lifebit-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifebit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 18:05:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloudos.lifebit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lifebit.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifebit-biotech/refs/heads/main/security/lifebit-biotech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Genomics
- Bioinformatics
- Federated Learning
- Trusted Research Environment
- Data Governance
- Life Sciences
- Sovereign AI
- OMOP
- Workflow Orchestration
---
