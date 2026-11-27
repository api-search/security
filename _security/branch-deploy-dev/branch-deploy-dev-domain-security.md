---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: branch-deploy.dev
  spf: true
hosts:
- cert_expires: Jan 17 20:48:09 2027 GMT
  host: branch-deploy.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BranchDeploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BranchDeploy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BranchDeploy
provider_slug: branch-deploy-dev
slug: branch-deploy-dev-domain-security
source_filename: branch-deploy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branch-deploy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 20:48:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: branch-deploy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/branch-deploy-dev/security/branch-deploy-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Microsoft Azure
- DevOps
- Deployment
- Automation
---
