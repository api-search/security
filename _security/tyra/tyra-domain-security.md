---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tyra.bio
  spf: true
hosts:
- cert_expires: Sep 16 04:25:40 2026 GMT
  host: tyra.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tyra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tyra Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tyra Biosciences
provider_slug: tyra
slug: tyra-domain-security
source_filename: tyra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tyra.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:25:40 2026 GMT\n  hsts: false\ndomains:\n- domain: tyra.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyra/refs/heads/main/security/tyra-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Precision Medicine
- Drug Discovery
- Oncology
- Therapeutics
- Life Sciences
---
