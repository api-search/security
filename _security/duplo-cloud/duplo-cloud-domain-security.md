---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: duplocloud.com
  spf: true
hosts:
- cert_expires: Aug 24 04:06:00 2026 GMT
  host: duplocloud.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duplo Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duplo Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Duplo Cloud
provider_slug: duplo-cloud
slug: duplo-cloud-domain-security
source_filename: duplo-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duplocloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:06:00 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: duplocloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duplo-cloud/refs/heads/main/security/duplo-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DevOps
- Cloud Infrastructure
- Infrastructure as Code
- Security and Compliance
- AI Agents
- Kubernetes
- Automation
---
