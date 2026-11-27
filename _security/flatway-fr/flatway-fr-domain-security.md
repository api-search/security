---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: flatway.fr
  spf: true
hosts:
- cert_expires: Jan  4 07:41:05 2027 GMT
  host: flatway.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flatway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flatway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Flatway
provider_slug: flatway-fr
slug: flatway-fr-domain-security
source_filename: flatway-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatway.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 07:41:05 2027 GMT\n  hsts: false\ndomains:\n- domain: flatway.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flatway-fr/security/flatway-fr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---
