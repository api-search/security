---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: scene.health
  spf: true
hosts:
- cert_expires: Oct  2 16:29:29 2026 GMT
  host: www.scene.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scene Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scene Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Scene Health
provider_slug: scene-health
slug: scene-health-domain-security
source_filename: scene-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scene.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:29:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scene.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scene-health/refs/heads/main/security/scene-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Medication Adherence
- Patient Engagement
- Telehealth
- Medicaid
- Public Health
- Clinical Trials
---
