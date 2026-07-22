---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thyrocare.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: thyrocare.cloud
  spf: false
hosts:
- cert_expires: Sep 16 01:06:37 2026 GMT
  host: thyrocare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: techso.thyrocare.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thyrocare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thyrocare, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thyrocare
provider_slug: thyrocare
slug: thyrocare-domain-security
source_filename: thyrocare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thyrocare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:06:37 2026 GMT\n  hsts: null\n- host: techso.thyrocare.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thyrocare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thyrocare.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thyrocare/refs/heads/main/security/thyrocare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Diagnostics
- Laboratory
- Pathology
- Preventive Care
- India
---
