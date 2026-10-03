---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bayzat.com
  spf: true
hosts:
- cert_expires: Oct 31 10:37:10 2026 GMT
  host: www.bayzat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bayzat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bayzat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bayzat
provider_slug: bayzat
slug: bayzat-domain-security
source_filename: bayzat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bayzat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:37:10 2026 GMT\n  hsts: false\ndomains:\n- domain: bayzat.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayzat/refs/heads/main/security/bayzat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Human Resources
- Payroll
- Benefits
- Software-as-a-Service
- GCC
---
