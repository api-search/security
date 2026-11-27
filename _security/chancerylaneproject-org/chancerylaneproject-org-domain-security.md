---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chancerylaneproject.org
  spf: true
hosts:
- cert_expires: Jan 20 20:17:59 2027 GMT
  host: chancerylaneproject.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Chancery Lane Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Chancery Lane Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Chancery Lane Project
provider_slug: chancerylaneproject-org
slug: chancerylaneproject-org-domain-security
source_filename: chancerylaneproject-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chancerylaneproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 20:17:59 2027 GMT\n  hsts: false\ndomains:\n- domain: chancerylaneproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chancerylaneproject-org/security/chancerylaneproject-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Charity
- Climate
- Sustainability
- Legal Tech
- Non-Profit
---
