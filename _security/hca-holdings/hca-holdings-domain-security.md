---
description: ''
domains:
- caa:
  - 128 issuewild "digicert.com"
  - 128 issuewild "awstrust.com"
  - 0 issue "pki.goog"
  - 128 issue "awstrust.com"
  - 128 issuewild "identrust.com"
  - 128 issue "identrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hcahealthcare.com
  spf: true
hosts:
- cert_expires: Dec 13 14:52:44 2026 GMT
  host: hcahealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hca Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HCA Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HCA Holdings
provider_slug: hca-holdings
slug: hca-holdings-domain-security
source_filename: hca-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hcahealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 14:52:44 2026 GMT\n  hsts: false\ndomains:\n- domain: hcahealthcare.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 128 issue \"awstrust.com\"\n  - 128 issuewild \"identrust.com\"\n  - 128 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hca-holdings/refs/heads/main/security/hca-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Hospitals
- Medical
- Health Systems
- Alias
- Fortune 100
---
