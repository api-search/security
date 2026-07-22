---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelml.com
  spf: true
hosts:
- cert_expires: Aug 27 12:56:03 2026 GMT
  host: www.modelml.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Model Ml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Model ML, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Model ML
provider_slug: model-ml
slug: model-ml-domain-security
source_filename: model-ml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modelml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: modelml.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/model-ml/refs/heads/main/security/model-ml-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Artificial Intelligence
- Financial Services
- AI Agents
- Investment Banking
- Enterprise
- Document Automation
---
