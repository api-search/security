---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dualentry.com
  spf: true
hosts:
- cert_expires: Sep 24 16:01:38 2026 GMT
  host: www.dualentry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:08:09 2026 GMT
  host: docs.dualentry.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.dualentry.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dualentry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DualEntry, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DualEntry
provider_slug: dualentry
slug: dualentry-domain-security
source_filename: dualentry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dualentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dualentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:08:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dualentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dualentry.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dualentry/refs/heads/main/security/dualentry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Accounting
- ERP
- Finance
- Financial Operations
- Bookkeeping
- Revenue Recognition
- Fintech
---
