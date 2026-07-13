---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudchipr.com
  spf: true
hosts:
- cert_expires: Aug 16 13:39:46 2026 GMT
  host: cloudchipr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:11:04 2026 GMT
  host: docs.cloudchipr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudchipr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudChipr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CloudChipr
provider_slug: cloudchipr
slug: cloudchipr-domain-security
source_filename: cloudchipr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudchipr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloudchipr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudchipr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/security/cloudchipr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Azure
- Cloud Cost Management
- Cost Optimization
- FinOps
- GCP
- Multi-Cloud
- Resource Cleanup
- Rightsizing
---
