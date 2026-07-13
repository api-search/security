---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cloudeagle.ai
  spf: true
hosts:
- cert_expires: Aug 31 20:55:03 2026 GMT
  host: www.cloudeagle.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudeagle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudEagle.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CloudEagle.ai
provider_slug: cloudeagle
slug: cloudeagle-domain-security
source_filename: cloudeagle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudeagle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:55:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudeagle.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudeagle/refs/heads/main/security/cloudeagle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Governance
- Cost Optimization
- License Management
- Procurement
- SaaS Management
- Shadow AI
- Shadow IT
- Software Procurement
- Vendor Management
---
