---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sofi.com
  spf: true
hosts:
- cert_expires: Dec  8 23:40:23 2026 GMT
  host: www.sofi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sofi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SoFi
provider_slug: sofi
slug: sofi-domain-security
source_filename: sofi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:40:23 2026 GMT\n  hsts: null\ndomains:\n- domain: sofi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi/refs/heads/main/security/sofi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Personal Finance
- Banking
- Lending
- Student Loans
- Mortgages
- Investing
- Credit Cards
- Fintech
- Open Banking
- Digital Banking
---
