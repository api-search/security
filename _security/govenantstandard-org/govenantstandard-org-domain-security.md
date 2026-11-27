---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: govenantstandard.org
  spf: true
hosts:
- cert_expires: Feb  8 03:51:50 2027 GMT
  host: govenantstandard.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GOVENANT Standard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GOVENANT Standard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GOVENANT Standard
provider_slug: govenantstandard-org
slug: govenantstandard-org-domain-security
source_filename: govenantstandard-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govenantstandard.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 03:51:50 2027 GMT\n  hsts: false\ndomains:\n- domain: govenantstandard.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/govenantstandard-org/security/govenantstandard-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Governance
- Standards
- Open Source
- Trust
---
