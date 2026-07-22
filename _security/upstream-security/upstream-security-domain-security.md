---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upstream.auto
  spf: true
hosts:
- cert_expires: Aug 28 05:21:20 2026 GMT
  host: upstream.auto
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upstream Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upstream Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upstream Security
provider_slug: upstream-security
slug: upstream-security-domain-security
source_filename: upstream-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upstream.auto\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upstream.auto\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstream-security/refs/heads/main/security/upstream-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Automotive
- Connected Vehicles
- Mobility
- IoT
- Threat Intelligence
---
