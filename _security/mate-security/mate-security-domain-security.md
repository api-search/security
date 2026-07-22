---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mate.security
  spf: true
hosts:
- cert_expires: Oct  6 18:23:45 2026 GMT
  host: mate.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mate Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mate Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mate Security
provider_slug: mate-security
slug: mate-security-domain-security
source_filename: mate-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mate.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mate.security\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mate-security/refs/heads/main/security/mate-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security
- Security Operations
- SOC
- Artificial Intelligence
- Threat Detection
- Incident Response
---
