---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vonlabs.ai
  spf: true
hosts:
- cert_expires: Oct 27 23:22:18 2026 GMT
  host: vonlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Von Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Von, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Von
provider_slug: von
slug: von-domain-security
source_filename: von-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vonlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:22:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vonlabs.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/von/refs/heads/main/security/von-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Revenue Operations
- Sales
- CRM
- Analytics
- Software-as-a-Service
---
