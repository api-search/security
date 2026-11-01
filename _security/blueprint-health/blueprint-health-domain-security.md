---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blueprint-health.com
  spf: true
hosts:
- cert_expires: Dec 19 01:12:42 2026 GMT
  host: blueprint-health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blueprint Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueprint Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blueprint Health
provider_slug: blueprint-health
slug: blueprint-health-domain-security
source_filename: blueprint-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueprint-health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blueprint-health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blueprint-health/security/blueprint-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HealthTech
- AI
- Therapy
- SaaS
- MentalHealth
---
