---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autorabit.com
  spf: true
hosts:
- cert_expires: Oct 29 15:15:31 2026 GMT
  host: www.autorabit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autorabit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoRABIT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AutoRABIT
provider_slug: autorabit
slug: autorabit-domain-security
source_filename: autorabit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autorabit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 15:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: autorabit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autorabit/refs/heads/main/security/autorabit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Salesforce
- DevSecOps
- CI/CD
- Compliance
- Automation
---
