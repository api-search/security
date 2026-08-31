---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: osmind.org
  spf: true
hosts:
- cert_expires: Oct  1 09:01:39 2026 GMT
  host: www.osmind.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osmind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Osmind
provider_slug: osmind
slug: osmind-domain-security
source_filename: osmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osmind.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osmind.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmind/refs/heads/main/security/osmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Psychiatry
- Electronic Health Records
- EHR
- Behavioral Health
- Digital Health
- HealthTech
---
