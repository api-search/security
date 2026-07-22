---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elevate.bio
  spf: true
hosts:
- cert_expires: Sep 14 21:35:05 2026 GMT
  host: www.elevate.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elevatebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ElevateBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ElevateBio
provider_slug: elevatebio
slug: elevatebio-domain-security
source_filename: elevatebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elevate.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:35:05 2026 GMT\n  hsts: false\ndomains:\n- domain: elevate.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevatebio/refs/heads/main/security/elevatebio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Tech
- Cell and Gene Therapy
- Biotechnology
- CDMO
- Genetic Medicine
- Manufacturing
- Life Sciences
---
