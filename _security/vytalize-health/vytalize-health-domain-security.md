---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vytalizehealth.com
  spf: true
hosts:
- cert_expires: Oct 17 18:28:45 2026 GMT
  host: www.vytalizehealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vytalize Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vytalize Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vytalize Health
provider_slug: vytalize-health
slug: vytalize-health-domain-security
source_filename: vytalize-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vytalizehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vytalizehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vytalize-health/refs/heads/main/security/vytalize-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Value Based Care
- Accountable Care Organization
- Medicare
- Population Health
- Clinical Decision Support
- Care Management
- Health Data
---
