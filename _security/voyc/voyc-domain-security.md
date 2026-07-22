---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voyc.ai
  spf: true
hosts:
- cert_expires: Sep  9 07:01:17 2026 GMT
  host: voyc.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voyc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Voyc
provider_slug: voyc
slug: voyc-domain-security
source_filename: voyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:01:17 2026 GMT\n  hsts: false\ndomains:\n- domain: voyc.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyc/refs/heads/main/security/voyc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversation Intelligence
- Compliance
- Call Monitoring
- Speech Analytics
- Contact Centers
- Financial Services
- Artificial Intelligence
---
