---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: revolv3.com
  spf: true
hosts:
- cert_expires: Jan 16 04:51:08 2027 GMT
  host: www.revolv3.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Revolv3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolv3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Revolv3
provider_slug: revolv3
slug: revolv3-domain-security
source_filename: revolv3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revolv3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 04:51:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: revolv3.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/revolv3/security/revolv3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- SaaS
- Enterprise
- API
---
