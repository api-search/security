---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gtisoft.com
  spf: true
hosts:
- cert_expires: Sep 20 12:54:23 2026 GMT
  host: www.gtisoft.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamma Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gamma Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gamma Technologies
provider_slug: gamma-technologies
slug: gamma-technologies-domain-security
source_filename: gamma-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gtisoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: gtisoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamma-technologies/refs/heads/main/security/gamma-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Simulation
- Engineering Software
- CAE
- Multiphysics
- Digital Twin
- Automotive
---
