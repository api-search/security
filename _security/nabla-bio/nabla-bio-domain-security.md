---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nabla.bio
  spf: false
hosts:
- cert_expires: Nov  1 00:25:26 2026 GMT
  host: www.nabla.bio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nabla Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nabla Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nabla Bio
provider_slug: nabla-bio
slug: nabla-bio-domain-security
source_filename: nabla-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nabla.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 00:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nabla.bio\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabla-bio/refs/heads/main/security/nabla-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Drug Discovery
- Protein Design
- Artificial Intelligence
- Machine-Learning
- Antibodies
- Generative Models
- Pharmaceuticals
---
