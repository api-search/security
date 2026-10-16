---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vitrolife.com
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: www.vitrolife.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vitrolife Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitrolife, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vitrolife
provider_slug: vitrolife
slug: vitrolife-domain-security
source_filename: vitrolife-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vitrolife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: vitrolife.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitrolife/refs/heads/main/security/vitrolife-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- IVF
- ReproductiveTechnology
- MedicalDevices
---
