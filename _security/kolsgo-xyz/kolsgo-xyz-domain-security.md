---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kolsgo.xyz
  spf: true
hosts:
- cert_expires: Feb  8 18:45:04 2027 GMT
  host: kolsgo.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kolsgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kolsgo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kolsgo
provider_slug: kolsgo-xyz
slug: kolsgo-xyz-domain-security
source_filename: kolsgo-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kolsgo.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 18:45:04 2027 GMT\n  hsts: false\ndomains:\n- domain: kolsgo.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kolsgo-xyz/security/kolsgo-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gaming
- Free
- Browser
- HTML5
- Community
---
