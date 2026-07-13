---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@landlordstudio.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: landlordstudio.com
  spf: true
hosts:
- cert_expires: Oct  1 07:56:35 2026 GMT
  host: www.landlordstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: portal.landlordstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landlordstudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landlord Studio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Landlord Studio
provider_slug: landlordstudio
slug: landlordstudio-domain-security
source_filename: landlordstudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landlordstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:56:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.landlordstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: landlordstudio.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@landlordstudio.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landlordstudio/refs/heads/main/security/landlordstudio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Property Management
- Real Estate
- Rental Income
- Expense Tracking
- Tenant Screening
- Rent Collection
- Financial Reporting
- Accounting
- Making Tax Digital
- MTD
---
