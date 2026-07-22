---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comsol.com
  spf: true
hosts:
- cert_expires: Jan  2 13:02:48 2027 GMT
  host: www.comsol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comsol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COMSOL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: COMSOL
provider_slug: comsol
slug: comsol-domain-security
source_filename: comsol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comsol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 13:02:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: comsol.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comsol/refs/heads/main/security/comsol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Simulation
- Multiphysics
- Engineering
- CAE
- CAD
- Modeling
- Desktop Software
- Scripting
---
