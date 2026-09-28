---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: belong-health.com
  spf: true
hosts:
- cert_expires: Oct 31 01:23:46 2026 GMT
  host: belong-health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Belong Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belong Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Belong Health
provider_slug: belong-health
slug: belong-health-domain-security
source_filename: belong-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: belong-health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 01:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: belong-health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belong-health/refs/heads/main/security/belong-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Insurance
- Medicare
- Healthcare
- Platform
- Company
---
