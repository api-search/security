---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: red6ar.com
  spf: true
hosts:
- cert_expires: Sep  3 18:52:15 2026 GMT
  host: red6ar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red6 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red 6, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Red 6
provider_slug: red6
slug: red6-domain-security
source_filename: red6-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: red6ar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:52:15 2026 GMT\n  hsts: false\ndomains:\n- domain: red6ar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red6/refs/heads/main/security/red6-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Defense
- Aerospace
- Augmented Reality
- Simulation and Training
- Military Aviation
- Head Mounted Display
- Artificial Intelligence
---
