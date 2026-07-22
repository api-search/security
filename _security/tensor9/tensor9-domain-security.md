---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tensor9.com
  spf: true
hosts:
- cert_expires: Aug 22 22:15:53 2026 GMT
  host: www.tensor9.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensor9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tensor9, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tensor9
provider_slug: tensor9
slug: tensor9-domain-security
source_filename: tensor9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tensor9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:15:53 2026 GMT\n  hsts: false\ndomains:\n- domain: tensor9.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensor9/refs/heads/main/security/tensor9-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Deployment
- BYOC
- Cloud Portability
- Infrastructure as Code
- Kubernetes
- On-Premises
- Security
- DevOps
- CLI
---
