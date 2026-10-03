---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aunalytics.com
  spf: true
hosts:
- cert_expires: Nov 20 07:30:42 2026 GMT
  host: www.aunalytics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aunalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aunalytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aunalytics
provider_slug: aunalytics
slug: aunalytics-domain-security
source_filename: aunalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aunalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 07:30:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: aunalytics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aunalytics/refs/heads/main/security/aunalytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Financial Services
- Data Analytics
- Cloud
---
