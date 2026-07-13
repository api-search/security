---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: grip.security
  spf: true
hosts:
- cert_expires: Sep 28 22:50:25 2026 GMT
  host: www.grip.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grip Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grip Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Grip Security
provider_slug: grip-security
slug: grip-security-domain-security
source_filename: grip-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.grip.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:50:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grip.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grip-security/refs/heads/main/security/grip-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Governance
- SaaS Security
---
