---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aucadastre.fr
  spf: true
hosts:
- cert_expires: Dec  3 09:28:48 2026 GMT
  host: aucadastre.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aucadastre Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aucadastre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aucadastre
provider_slug: aucadastre-fr
slug: aucadastre-fr-domain-security
source_filename: aucadastre-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aucadastre.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 09:28:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aucadastre.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aucadastre-fr/security/aucadastre-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- cadastre
- urbanisme
- Geospatial
- France
- Public Data
---
