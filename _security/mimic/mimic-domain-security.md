---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mimic.com
  spf: true
hosts:
- cert_expires: Aug 28 20:09:45 2026 GMT
  host: mimic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mimic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mimic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mimic
provider_slug: mimic
slug: mimic-domain-security
source_filename: mimic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mimic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:09:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mimic.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mimic/refs/heads/main/security/mimic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Ransomware Defense
- Endpoint Security
- Threat Detection
- AI Security
- SaaS
---
