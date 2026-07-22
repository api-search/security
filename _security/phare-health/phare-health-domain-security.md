---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: phare.health
  spf: true
hosts:
- cert_expires: Sep 20 16:17:50 2026 GMT
  host: phare.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phare Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phare Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Phare Health
provider_slug: phare-health
slug: phare-health-domain-security
source_filename: phare-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phare.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:17:50 2026 GMT\n  hsts: false\ndomains:\n- domain: phare.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phare-health/refs/heads/main/security/phare-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Medical Coding
- Clinical Documentation
- Artificial Intelligence
- Health IT
---
