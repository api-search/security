---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heathy.org
  spf: true
hosts:
- cert_expires: Jan  8 16:47:00 2027 GMT
  host: heathy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heathy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heathy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Heathy
provider_slug: heathy-org
slug: heathy-org-domain-security
source_filename: heathy-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heathy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 16:47:00 2027 GMT\n  hsts: false\ndomains:\n- domain: heathy.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heathy-org/security/heathy-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Nutrition
- Food Data
- Health
- Open Data
---
