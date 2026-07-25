---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gitops.tech
  spf: true
hosts:
- cert_expires: Sep 25 00:04:51 2026 GMT
  host: www.gitops.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitOps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GitOps
provider_slug: gitops
slug: gitops-domain-security
source_filename: gitops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gitops.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:04:51 2026 GMT\n  hsts: false\ndomains:\n- domain: gitops.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitops/refs/heads/main/security/gitops-domain-security.yml
summary_line: TLSv1.3
tags:
- Automation
- Continuous Deployment
- DevOps
- Infrastructure as Code
- Version Control
---
