---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: glyphic.bio
  spf: true
hosts:
- cert_expires: Sep 25 04:28:49 2026 GMT
  host: glyphic.bio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glyphic Biotechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glyphic Biotechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Glyphic Biotechnologies
provider_slug: glyphic-biotechnologies
slug: glyphic-biotechnologies-domain-security
source_filename: glyphic-biotechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glyphic.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: glyphic.bio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glyphic-biotechnologies/refs/heads/main/security/glyphic-biotechnologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Proteomics
- Protein Sequencing
- Biotechnology
- Life Sciences
- Single-Molecule Sequencing
- Drug Discovery
---
