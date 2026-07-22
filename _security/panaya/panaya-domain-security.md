---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: panaya.com
  spf: true
hosts:
- cert_expires: Oct 16 14:59:35 2026 GMT
  host: www.panaya.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 11:26:58 2026 GMT
  host: success.panaya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: my.panaya.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panaya, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Panaya
provider_slug: panaya
slug: panaya-domain-security
source_filename: panaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.panaya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: success.panaya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:26:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.panaya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: panaya.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panaya/refs/heads/main/security/panaya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Testing
- Test Automation
- Test Management
- Change Management
- Change Impact Analysis
- ERP
- SAP
- Oracle
- Salesforce
- Quality Assurance
- DevOps
---
