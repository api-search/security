---
api_specs:
- filename: git.json
  format: json
  label: Azure DevOps Services REST API - Git
  slug: azure-devops-services-rest-api-git
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/git/7.1/git.json
- filename: tfvc.json
  format: json
  label: Azure DevOps Services REST API - TFVC
  slug: azure-devops-services-rest-api-tfvc
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/tfvc/7.1/tfvc.json
- filename: policy.json
  format: json
  label: Azure DevOps Services REST API - Policy
  slug: azure-devops-services-rest-api-policy
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/policy/7.1/policy.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Repo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Repos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Repos
provider_slug: microsoft-azure-repo
slug: microsoft-azure-repo-domain-security
source_filename: microsoft-azure-repo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/security/microsoft-azure-repo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- Git
- Repositories
- Source Control
- TFVC
- Version Control
---
