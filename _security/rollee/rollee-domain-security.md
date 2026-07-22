---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "zerossl.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getrollee.com
  spf: true
hosts:
- cert_expires: Oct  6 09:53:49 2026 GMT
  host: www.getrollee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:04:23 2026 GMT
  host: developers.getrollee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 08:51:18 2026 GMT
  host: api.getrollee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rollee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rollee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rollee
provider_slug: rollee
slug: rollee-domain-security
source_filename: rollee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:53:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:04:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:51:18 2026 GMT\n  hsts: null\ndomains:\n- domain: getrollee.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"zerossl.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/security/rollee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Open Finance
- Income Verification
- Employment Verification
- Payroll Data
- Gig Economy
- Alternative Data
- Underwriting
- Lending
- Fintech
---
