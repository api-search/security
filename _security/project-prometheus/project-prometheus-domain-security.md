---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prometheus.ai
  spf: true
hosts:
- cert_expires: Sep  9 12:14:37 2026 GMT
  host: www.prometheus.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Project Prometheus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Project Prometheus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Project Prometheus
provider_slug: project-prometheus
slug: project-prometheus-domain-security
source_filename: project-prometheus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prometheus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:14:37 2026 GMT\n  hsts: null\ndomains:\n- domain: prometheus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project-prometheus/refs/heads/main/security/project-prometheus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Physical AI
- Machine-Learning
- Manufacturing
- Aerospace
- Engineering
- Stealth
---
