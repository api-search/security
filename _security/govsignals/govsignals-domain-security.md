---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: govsignals.ai
  spf: true
hosts:
- cert_expires: Jan  9 16:38:33 2027 GMT
  host: www.govsignals.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Govsignals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovSignals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GovSignals
provider_slug: govsignals
slug: govsignals-domain-security
source_filename: govsignals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govsignals.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:38:33 2027 GMT\n  hsts: false\ndomains:\n- domain: govsignals.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/govsignals/security/govsignals-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI
- Procurement
- Government
- Platform
---
