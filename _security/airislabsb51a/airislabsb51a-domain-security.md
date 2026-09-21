---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airis-labs.com
  spf: true
hosts:
- cert_expires: Dec 13 23:05:32 2026 GMT
  host: www.airis-labs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airislabsb51A Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airis Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airis Labs
provider_slug: airislabsb51a
slug: airislabsb51a-domain-security
source_filename: airislabsb51a-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airis-labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:05:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airis-labs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airislabsb51a/refs/heads/main/security/airislabsb51a-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Homeland Security
- Public Safety
- Video Intelligence
- Computer-Vision
- Artificial Intelligence
- Intelligence Analysis
- Agentic AI
---
