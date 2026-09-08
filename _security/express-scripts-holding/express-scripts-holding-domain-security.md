---
description: ''
domains:
- caa:
  - 128 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "cloudflare.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: express-scripts.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.express-scripts.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Verified directly on 2026-09-07 with a browser User-Agent: `strict-transport-security: max-age=31536000; includeSubDomains`. The automated sweep recorded null on this run; that was a false negative and is corrected here rather than left to under-credit the provider.'
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Express Scripts Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Express Scripts Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Express Scripts Holding
provider_slug: express-scripts-holding
slug: express-scripts-holding-domain-security
source_filename: express-scripts-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.express-scripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Verified directly on 2026-09-07 with a browser User-Agent:\n    `strict-transport-security: max-age=31536000; includeSubDomains`.\n    The automated sweep recorded null on this run; that was a false negative and is\n    corrected here rather than left to under-credit the provider.\ndomains:\n- domain: express-scripts.com\n  dnssec: true\n  caa:\n  - 128 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"cloudflare.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-scripts-holding/refs/heads/main/security/express-scripts-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Healthcare
- Pharmacy
- Pharmacy Benefit Management
- Prescriptions
- Claims
- Fortune 100
---
