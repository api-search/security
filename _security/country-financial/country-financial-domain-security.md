---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: countryfinancial.com
  spf: true
hosts:
- cert_expires: Aug 19 07:05:32 2026 GMT
  host: www.countryfinancial.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Country Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COUNTRY Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: COUNTRY Financial
provider_slug: country-financial
slug: country-financial-domain-security
source_filename: country-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.countryfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:05:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: countryfinancial.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-financial/refs/heads/main/security/country-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agribusiness
- Auto Insurance
- Bloomington
- Commercial Insurance
- Crop Insurance
- Farm Insurance
- Financial Services
- Home Insurance
- Illinois
- Insurance
- Investments
- Life Insurance
- Mutual Insurance
- Retirement Planning
- Trust Services
---
