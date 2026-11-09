---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: calculpro.fr
  spf: true
hosts:
- cert_expires: Jan 28 17:06:43 2027 GMT
  host: calculpro.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calculpro Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CalculPro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CalculPro
provider_slug: calculpro-fr
slug: calculpro-fr-domain-security
source_filename: calculpro-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calculpro.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 17:06:43 2027 GMT\n  hsts: false\ndomains:\n- domain: calculpro.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/calculpro-fr/security/calculpro-fr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Construction
- Engineering
- Calculators
- BuildingTools
- FrenchStandards
---
