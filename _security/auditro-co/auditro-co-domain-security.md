---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: auditro.co
  spf: true
hosts:
- cert_expires: Jan 14 06:28:35 2027 GMT
  host: auditro.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auditro Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auditro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Auditro
provider_slug: auditro-co
slug: auditro-co-domain-security
source_filename: auditro-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auditro.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:28:35 2027 GMT\n  hsts: null\ndomains:\n- domain: auditro.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/auditro-co/security/auditro-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ICV
- Emiratisation
- Procurement
- Finance
- Human Resources
- United Arab Emirates
- Score Planning
---
