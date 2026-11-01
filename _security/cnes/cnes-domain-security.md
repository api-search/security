---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cnes.fr
  spf: true
hosts:
- cert_expires: Dec 20 19:41:24 2026 GMT
  host: www.cnes.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cnes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNES, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CNES
provider_slug: cnes
slug: cnes-domain-security
source_filename: cnes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnes.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 19:41:24 2026 GMT\n  hsts: null\ndomains:\n- domain: cnes.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cnes/security/cnes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
