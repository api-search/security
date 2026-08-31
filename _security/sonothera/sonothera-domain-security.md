---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonothera.com
  spf: true
hosts:
- cert_expires: Nov 26 10:27:52 2026 GMT
  host: sonothera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonothera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SonoThera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SonoThera
provider_slug: sonothera
slug: sonothera-domain-security
source_filename: sonothera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sonothera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 10:27:52 2026 GMT\n  hsts: false\ndomains:\n- domain: sonothera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonothera/refs/heads/main/security/sonothera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Gene Therapy
- Genetic Medicine
- Drug Delivery
- Ultrasound
- Life Sciences
- Clinical Trials
- Rare Disease
---
