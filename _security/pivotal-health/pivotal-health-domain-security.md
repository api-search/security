---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pivotalhealth.ai
  spf: true
hosts:
- cert_expires: Oct  3 05:22:15 2026 GMT
  host: pivotalhealth.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pivotal Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pivotal Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pivotal Health
provider_slug: pivotal-health
slug: pivotal-health-domain-security
source_filename: pivotal-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pivotalhealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:22:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pivotalhealth.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pivotal-health/refs/heads/main/security/pivotal-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Independent Dispute Resolution
- No Surprises Act
- Reimbursement
- Insurance Claims
- Health Tech
---
