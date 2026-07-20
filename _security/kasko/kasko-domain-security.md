---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:sysarch@kasko.io"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kasko.io
  spf: true
hosts:
- cert_expires: Sep  7 08:36:48 2026 GMT
  host: kasko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kasko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kasko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kasko
provider_slug: kasko
slug: kasko-domain-security
source_filename: kasko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kasko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:36:48 2026 GMT\n  hsts: null\ndomains:\n- domain: kasko.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:sysarch@kasko.io\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kasko/refs/heads/main/security/kasko-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- InsurTech
- Insurance API
- Policy Management
- Payments
- Webhooks
- Embedded Insurance
- No-Code
---
