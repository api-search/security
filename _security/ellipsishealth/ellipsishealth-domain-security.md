---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ellipsishealth.com
  spf: true
hosts:
- cert_expires: Sep  2 19:38:48 2026 GMT
  host: www.ellipsishealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ellipsishealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ellipsis Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ellipsis Health
provider_slug: ellipsishealth
slug: ellipsishealth-domain-security
source_filename: ellipsishealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ellipsishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 19:38:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ellipsishealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsishealth/refs/heads/main/security/ellipsishealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Artificial Intelligence
- Vocal Biomarkers
- Voice AI
- Digital Health
- Care Management
- HIPAA
---
