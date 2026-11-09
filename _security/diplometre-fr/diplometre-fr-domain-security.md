---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: diplometre.fr
  spf: true
hosts:
- cert_expires: Jan  3 05:14:14 2027 GMT
  host: diplometre.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diplometre Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diplomètre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Diplomètre
provider_slug: diplometre-fr
slug: diplometre-fr-domain-security
source_filename: diplometre-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diplometre.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:14:14 2027 GMT\n  hsts: null\ndomains:\n- domain: diplometre.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/diplometre-fr/security/diplometre-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Orientation
- Parents
---
