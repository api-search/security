---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bamboohealth.com
  spf: true
hosts:
- cert_expires: Sep 13 02:57:31 2026 GMT
  host: bamboohealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bamboo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bamboo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bamboo Health
provider_slug: bamboo-health
slug: bamboo-health-domain-security
source_filename: bamboo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bamboohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:57:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bamboohealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboo-health/refs/heads/main/security/bamboo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Care Coordination
- Behavioral Health
- Prescription Drug Monitoring
- PDMP
- Health IT
- Interoperability
---
