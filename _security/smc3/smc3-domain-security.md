---
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 issue "godaddy.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smc3.com
  spf: true
hosts:
- cert_expires: Jan 10 19:17:25 2027 GMT
  host: smc3.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SMC3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMC3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SMC3
provider_slug: smc3
slug: smc3-domain-security
source_filename: smc3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smc3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 19:17:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smc3.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/smc3/security/smc3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Transportation
- Pricing
---
