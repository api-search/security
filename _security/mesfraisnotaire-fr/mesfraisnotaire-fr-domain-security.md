---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mesfraisnotaire.fr
  spf: true
hosts:
- cert_expires: Feb  8 10:09:19 2027 GMT
  host: mesfraisnotaire.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mes Frais de Notaire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mes Frais de Notaire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mes Frais de Notaire
provider_slug: mesfraisnotaire-fr
slug: mesfraisnotaire-fr-domain-security
source_filename: mesfraisnotaire-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mesfraisnotaire.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 10:09:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mesfraisnotaire.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mesfraisnotaire-fr/security/mesfraisnotaire-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Notary
- Real Estate
- France
- Calculator
---
