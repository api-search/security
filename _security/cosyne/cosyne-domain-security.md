---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cosyne.com
  spf: true
hosts:
- cert_expires: Jan 25 14:14:48 2027 GMT
  host: www.cosyne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cosyne
provider_slug: cosyne
slug: cosyne-domain-security
source_filename: cosyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 14:14:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cosyne/security/cosyne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- DrugDiscovery
- PrecisionMedicine
- BrainCancer
---
