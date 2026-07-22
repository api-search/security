---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pothlabs.com
  spf: true
hosts:
- cert_expires: Oct 11 20:14:18 2026 GMT
  host: pothlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poth Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poth Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Poth Labs
provider_slug: poth-labs
slug: poth-labs-domain-security
source_filename: poth-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pothlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:14:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pothlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poth-labs/refs/heads/main/security/poth-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- SaaS
- Customer Research
- Market Research
- Customer Feedback
- Analytics
- B2B
- Workflow Automation
---
