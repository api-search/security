---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "edicomgroup.com"
  - 0 issue "edicomgroup.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edicomgroup.com
  spf: true
hosts:
- cert_expires: Dec 28 09:47:48 2026 GMT
  host: edicomgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edicom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edicom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edicom
provider_slug: edicom
slug: edicom-domain-security
source_filename: edicom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edicomgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 09:47:48 2026 GMT\n  hsts: false\ndomains:\n- domain: edicomgroup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"edicomgroup.com\"\n  - 0 issue \"edicomgroup.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/edicom/security/edicom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EDI
- E-Invoicing
- Tax Compliance
- B2B Integration
- iPaaS
- VAT Reporting
- PEPPOL
---
