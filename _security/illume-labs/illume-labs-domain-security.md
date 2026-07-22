---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: illumelabs.ai
  spf: true
hosts:
- cert_expires: Sep 25 00:39:27 2026 GMT
  host: www.illumelabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Illume Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Illume Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Illume Labs
provider_slug: illume-labs
slug: illume-labs-domain-security
source_filename: illume-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.illumelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:39:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: illumelabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/illume-labs/refs/heads/main/security/illume-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Health
- Longevity
- Wearables
- Genomics
- Digital Health
- Consumer Health
- Personalized Medicine
---
