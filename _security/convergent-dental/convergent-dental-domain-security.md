---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convergentdental.com
  spf: true
hosts:
- cert_expires: Sep 21 08:26:58 2026 GMT
  host: www.convergentdental.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convergent Dental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convergent Dental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Convergent Dental
provider_slug: convergent-dental
slug: convergent-dental-domain-security
source_filename: convergent-dental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convergentdental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:26:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: convergentdental.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convergent-dental/refs/heads/main/security/convergent-dental-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Dental
- Healthcare
- Lasers
- Dental Equipment
- Manufacturing
- Clinical Technology
---
