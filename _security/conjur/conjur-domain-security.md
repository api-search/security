---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Conjur / CyberArk Secrets Manager API
  slug: conjur-cyberark-secrets-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conjur/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conjur.org
  spf: true
hosts:
- cert_expires: Sep 15 03:04:10 2026 GMT
  host: conjur.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conjur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conjur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conjur
provider_slug: conjur
slug: conjur-domain-security
source_filename: conjur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conjur.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:04:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conjur.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conjur/refs/heads/main/security/conjur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Secrets Management
- Identity and Access Management
- DevSecOps
- Kubernetes
- Machine Identity
- Open Source
---
