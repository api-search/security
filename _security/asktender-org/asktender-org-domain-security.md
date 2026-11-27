---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asktender.org
  spf: true
hosts:
- cert_expires: Jan 23 00:42:12 2027 GMT
  host: asktender.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: askTender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for askTender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: askTender
provider_slug: asktender-org
slug: asktender-org-domain-security
source_filename: asktender-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asktender.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 00:42:12 2027 GMT\n  hsts: false\ndomains:\n- domain: asktender.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/asktender-org/security/asktender-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Procurement
- Government
- B2B
- Software-as-a-Service
- Marketplace
---
