---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: limbic.ai
  spf: true
hosts:
- cert_expires: Oct 14 11:22:06 2026 GMT
  host: limbic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limbic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limbic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Limbic
provider_slug: limbic
slug: limbic-domain-security
source_filename: limbic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: limbic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:22:06 2026 GMT\n  hsts: false\ndomains:\n- domain: limbic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limbic/refs/heads/main/security/limbic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Artificial Intelligence
- Clinical Decision Support
- Digital Health
- Medical Devices
- Behavioral Health
- NHS
---
