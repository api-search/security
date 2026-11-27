---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aurentia.fr
  spf: true
hosts:
- cert_expires: Jan 23 09:28:53 2027 GMT
  host: aurentia.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurentia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurentia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aurentia
provider_slug: aurentia-fr
slug: aurentia-fr-domain-security
source_filename: aurentia-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurentia.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 09:28:53 2027 GMT\n  hsts: false\ndomains:\n- domain: aurentia.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aurentia-fr/security/aurentia-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Entrepreneurship
- Productivity
- Tools
- Platform
- Business
---
