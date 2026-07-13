---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skybiometry.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: skybiometry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skybiometry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkyBiometry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SkyBiometry
provider_slug: skybiometry
slug: skybiometry-domain-security
source_filename: skybiometry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skybiometry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: skybiometry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skybiometry/refs/heads/main/security/skybiometry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Learning
- Public APIs
---
