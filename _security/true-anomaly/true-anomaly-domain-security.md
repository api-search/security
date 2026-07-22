---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trueanomaly.space
  spf: true
hosts:
- cert_expires: Sep 18 15:20:37 2026 GMT
  host: www.trueanomaly.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: True Anomaly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for True Anomaly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: True Anomaly
provider_slug: true-anomaly
slug: true-anomaly-domain-security
source_filename: true-anomaly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trueanomaly.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:20:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trueanomaly.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-anomaly/refs/heads/main/security/true-anomaly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Defense
- Aerospace
- Autonomy
- Software
- National Security
- Spacecraft
---
