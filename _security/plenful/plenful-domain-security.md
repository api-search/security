---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "amazonwas.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plenful.com
  spf: true
hosts:
- cert_expires: Oct  3 10:55:44 2026 GMT
  host: www.plenful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plenful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plenful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plenful
provider_slug: plenful
slug: plenful-domain-security
source_filename: plenful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plenful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:55:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plenful.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"amazonwas.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plenful/refs/heads/main/security/plenful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Artificial Intelligence
- Workflow Automation
- Machine Learning
- 340B
- Prior Authorization
---
