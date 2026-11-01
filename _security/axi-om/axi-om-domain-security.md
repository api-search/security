---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axi.om
  spf: true
hosts:
- cert_expires: Dec 18 19:18:38 2026 GMT
  host: axi.om
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axi Om Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axiom
provider_slug: axi-om
slug: axi-om-domain-security
source_filename: axi-om-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axi.om\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 19:18:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: axi.om\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/axi-om/security/axi-om-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drug Toxicity Prediction
- Clinical Outcomes
- Medicinal Chemistry
---
