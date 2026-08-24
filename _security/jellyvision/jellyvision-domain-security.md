---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jellyvision.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myalex.com
  spf: true
hosts:
- cert_expires: Oct 18 20:10:19 2026 GMT
  host: www.jellyvision.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: partner-api-docs.myalex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.myalex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jellyvision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jellyvision, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jellyvision
provider_slug: jellyvision
slug: jellyvision-domain-security
source_filename: jellyvision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jellyvision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 20:10:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partner-api-docs.myalex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: www.myalex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jellyvision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myalex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jellyvision/refs/heads/main/security/jellyvision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Benefits
- Human Resources
- Benefits Administration
- Benefits Enrollment
- Health Insurance
- Decision Support
- HR Technology
- Insurance
- Employee Engagement
---
