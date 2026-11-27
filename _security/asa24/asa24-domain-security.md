---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cancer.gov
  spf: true
hosts:
- cert_expires: Dec 19 03:08:12 2026 GMT
  host: epi.grants.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ASA24 (NCI) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASA24 (NCI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ASA24 (NCI)
provider_slug: asa24
slug: asa24-domain-security
source_filename: asa24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epi.grants.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 03:08:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cancer.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/asa24/security/asa24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Dietary Assessment
- Nutrition
- Public Health
- Research
- Government
---
