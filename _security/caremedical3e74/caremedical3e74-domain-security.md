---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caremedga.com
  spf: true
hosts:
- cert_expires: Dec 20 03:07:06 2026 GMT
  host: caremedga.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caremedical3E74 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caremedical3e74, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caremedical3e74
provider_slug: caremedical3e74
slug: caremedical3e74-domain-security
source_filename: caremedical3e74-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caremedga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 03:07:06 2026 GMT\n  hsts: false\ndomains:\n- domain: caremedga.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caremedical3e74/refs/heads/main/security/caremedical3e74-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical
- Equipment
- HomeCare
- Georgia
---
