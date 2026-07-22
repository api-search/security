---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: authentic8.com
  spf: true
hosts:
- cert_expires: Sep 20 11:24:47 2026 GMT
  host: www.authentic8.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authentic8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authentic8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Authentic8
provider_slug: authentic8
slug: authentic8-domain-security
source_filename: authentic8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authentic8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:24:47 2026 GMT\n  hsts: false\ndomains:\n- domain: authentic8.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authentic8/refs/heads/main/security/authentic8-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Secure Browser
- Threat Intelligence
- Digital Investigations
- Managed Attribution
- Dark Web
---
