---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: beamline.io
  spf: true
hosts:
- cert_expires: Jan 10 09:29:49 2027 GMT
  host: beamline.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beamline UI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beamline UI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Beamline UI
provider_slug: beamline-io
slug: beamline-io-domain-security
source_filename: beamline-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beamline.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 09:29:49 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: beamline.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/beamline-io/security/beamline-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- UI
- React
- Components
- Software-as-a-Service
- Open Source
---
