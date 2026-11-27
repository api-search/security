---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foodnotes.org
  spf: true
hosts:
- cert_expires: Feb  6 10:22:37 2027 GMT
  host: foodnotes.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FoodNotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FoodNotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FoodNotes
provider_slug: foodnotes-org
slug: foodnotes-org-domain-security
source_filename: foodnotes-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foodnotes.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 10:22:37 2027 GMT\n  hsts: false\ndomains:\n- domain: foodnotes.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foodnotes-org/security/foodnotes-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nutrition
- Health
- Food
- Data
- Tools
---
