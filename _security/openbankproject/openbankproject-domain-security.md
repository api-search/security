---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openbankproject.com
  spf: true
hosts:
- cert_expires: Jan 10 17:47:27 2027 GMT
  host: openbankproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openbankproject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Bank Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Bank Project
provider_slug: openbankproject
slug: openbankproject-domain-security
source_filename: openbankproject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openbankproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 17:47:27 2027 GMT\n  hsts: false\ndomains:\n- domain: openbankproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openbankproject/security/openbankproject-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- OpenBanking
- API
- Fintech
- Banking
---
