---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monaire.ai
  spf: true
hosts:
- cert_expires: Jan 17 02:59:31 2027 GMT
  host: monaire.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monaire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monaire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Monaire
provider_slug: monaire
slug: monaire-domain-security
source_filename: monaire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monaire.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 02:59:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monaire.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/monaire/security/monaire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- HVAC
- EnergyManagement
- SaaS
---
