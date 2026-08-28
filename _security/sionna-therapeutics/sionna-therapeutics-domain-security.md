---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sionnatx.com
  spf: true
hosts:
- cert_expires: Nov  8 01:47:53 2026 GMT
  host: www.sionnatx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sionna Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sionna Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sionna Therapeutics
provider_slug: sionna-therapeutics
slug: sionna-therapeutics-domain-security
source_filename: sionna-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sionnatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 01:47:53 2026 GMT\n  hsts: false\ndomains:\n- domain: sionnatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sionna-therapeutics/refs/heads/main/security/sionna-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Drug Development
- Rare Disease
- Cystic Fibrosis
- Small Molecule
---
