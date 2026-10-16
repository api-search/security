---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cbtnuggets.com
  spf: true
hosts:
- cert_expires: Nov 14 05:40:05 2026 GMT
  host: www.cbtnuggets.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cbtnuggets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cbtnuggets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cbtnuggets
provider_slug: cbtnuggets
slug: cbtnuggets-domain-security
source_filename: cbtnuggets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbtnuggets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 05:40:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cbtnuggets.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cbtnuggets/refs/heads/main/security/cbtnuggets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- IT
- Training
- Video
- Certification
- Education
---
