---
api_specs:
- filename: kangaroo-rewards-core-api-openapi.yml
  format: yaml
  label: Kangaroo Rewards Core API
  slug: kangaroo-rewards-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kangaroo-rewards/refs/heads/main/openapi/kangaroo-rewards-core-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kangaroorewards.com
  spf: true
hosts:
- cert_expires: Dec 28 11:56:24 2026 GMT
  host: www.kangaroorewards.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kangaroo Rewards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kangaroo Rewards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kangaroo Rewards
provider_slug: kangaroo-rewards
slug: kangaroo-rewards-domain-security
source_filename: kangaroo-rewards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kangaroorewards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:56:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kangaroorewards.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kangaroo-rewards/refs/heads/main/security/kangaroo-rewards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Loyalty
- Marketing
- SaaS
- Rewards
---
