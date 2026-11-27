---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: facturacobra.com
  spf: true
hosts:
- host: facturacobra.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobra Punto de Venta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobra Punto de Venta, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cobra Punto de Venta
provider_slug: facturacobra-com
slug: facturacobra-com-domain-security
source_filename: facturacobra-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facturacobra.com\n  https: false\ndomains:\n- domain: facturacobra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/facturacobra-com/security/facturacobra-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
