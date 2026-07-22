---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eye.security
  spf: true
hosts:
- cert_expires: Oct 11 17:38:24 2026 GMT
  host: www.eye.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: portal.eye.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eye Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eye Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Eye Security
provider_slug: eye-security
slug: eye-security-domain-security
source_filename: eye-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eye.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:38:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.eye.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eye.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eye-security/refs/heads/main/security/eye-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Managed XDR
- Security Operations Center
- Incident Response
- Cyber Insurance
- Threat Hunting
- Europe
---
