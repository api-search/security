---
description: ''
domains:
- caa:
  - 0 issue "Sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "rapidssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finli.com
  spf: true
hosts:
- cert_expires: Sep  8 23:07:18 2026 GMT
  host: finli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finli
provider_slug: finli
slug: finli-domain-security
source_filename: finli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:07:18 2026 GMT\n  hsts: false\ndomains:\n- domain: finli.com\n  dnssec: false\n  caa:\n  - 0 issue \"Sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"rapidssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finli/refs/heads/main/security/finli-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Invoicing
- Small Business
- Billing
- Banking
- ACH
---
