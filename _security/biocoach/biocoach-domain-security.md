---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biocoach.health
  spf: true
hosts:
- cert_expires: Nov 19 23:55:21 2026 GMT
  host: biocoach.health
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biocoach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioCoach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BioCoach
provider_slug: biocoach
slug: biocoach-domain-security
source_filename: biocoach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biocoach.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:55:21 2026 GMT\n  hsts: false\ndomains:\n- domain: biocoach.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biocoach/refs/heads/main/security/biocoach-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- DigitalHealth
- Nutrition
- AI
- Longevity
- Company
---
