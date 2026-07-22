---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: collectivehealth.com
  spf: true
hosts:
- cert_expires: Oct  2 16:40:55 2026 GMT
  host: collectivehealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collective Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collective Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Collective Health
provider_slug: collective-health
slug: collective-health-domain-security
source_filename: collective-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collectivehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:40:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: collectivehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collective-health/refs/heads/main/security/collective-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Health Benefits
- Third-Party Administrator
- Health Insurance
- Healthcare
- Employee Benefits
---
