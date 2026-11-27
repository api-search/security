---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affine.earth
  spf: false
hosts:
- cert_expires: Jan 28 10:42:49 2027 GMT
  host: affine.earth
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Affine.Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affine.Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Affine.Earth
provider_slug: affine-earth
slug: affine-earth-domain-security
source_filename: affine-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affine.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:42:49 2027 GMT\n  hsts: false\ndomains:\n- domain: affine.earth\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/affine-earth/security/affine-earth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Quantum Computing
- Interactive IDE
- Scientific Simulations
- Open Source
---
