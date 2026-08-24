---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sail.bio
  spf: true
hosts:
- cert_expires: Sep 24 10:49:32 2026 GMT
  host: www.sail.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laronde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sail Biomedicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sail Biomedicines
provider_slug: laronde
slug: laronde-domain-security
source_filename: laronde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sail.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:49:32 2026 GMT\n  hsts: false\ndomains:\n- domain: sail.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laronde/refs/heads/main/security/laronde-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- RNA
- Circular RNA
- Cell Therapy
- CAR-T
- Nanoparticles
- Drug Discovery
- Immunology
- Autoimmune Disease
- Life Sciences
- Artificial Intelligence
- Preclinical
---
