---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marathon-health.com
  spf: true
hosts:
- cert_expires: Sep  7 20:23:25 2026 GMT
  host: www.marathon-health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marathon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marathon Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Marathon Health
provider_slug: marathon-health
slug: marathon-health-domain-security
source_filename: marathon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marathon-health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:23:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marathon-health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marathon-health/refs/heads/main/security/marathon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Primary Care
- Occupational Health
- Employer Health
- Population Health
- Telehealth
- Healthcare Services
---
