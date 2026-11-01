---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: subito.it
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: subito.it
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Subito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subito.it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Subito.it
provider_slug: subito
slug: subito-domain-security
source_filename: subito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: subito.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: subito.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/subito/security/subito-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketplace
- Classifieds
- E-commerce
- Italy
- Recommerce
---
