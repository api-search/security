---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soleranetwork.com
  spf: true
hosts:
- cert_expires: Feb  6 21:01:37 2027 GMT
  host: www.soleranetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 21:01:37 2027 GMT
  host: api.soleranetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solera Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solera Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solera Health
provider_slug: solera-health
slug: solera-health-domain-security
source_filename: solera-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soleranetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 21:01:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.soleranetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 21:01:37 2027 GMT\n  hsts: null\ndomains:\n- domain: soleranetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solera-health/refs/heads/main/security/solera-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Benefits
- Employee Benefits
- Health Plans
- Payer
- Provider Network
- Chronic Condition Management
- Preventive Care
- Telehealth
---
