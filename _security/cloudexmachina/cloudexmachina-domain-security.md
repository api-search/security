---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "google.com"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "google.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudexmachina.io
  spf: true
hosts:
- cert_expires: Oct  8 17:50:10 2026 GMT
  host: www.cloudexmachina.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudexmachina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Ex Machina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloud Ex Machina
provider_slug: cloudexmachina
slug: cloudexmachina-domain-security
source_filename: cloudexmachina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudexmachina.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:50:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudexmachina.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"google.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"google.com\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudexmachina/refs/heads/main/security/cloudexmachina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Cloud
- FinOps
- Cloud Cost Optimization
- Cloud Governance
- AI Agents
- Cloud Management
- Terraform
- Kubernetes
---
