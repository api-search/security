---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: behavox.com
  spf: true
hosts:
- cert_expires: Oct 14 12:41:05 2026 GMT
  host: behavox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Behavox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Behavox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Behavox
provider_slug: behavox
slug: behavox-domain-security
source_filename: behavox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: behavox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:41:05 2026 GMT\n  hsts: false\ndomains:\n- domain: behavox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/behavox/refs/heads/main/security/behavox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Compliance
- Surveillance
- RegTech
- Artificial Intelligence
- Financial Services
- Security
---
