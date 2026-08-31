---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentacenter.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acima.com
  spf: true
hosts:
- cert_expires: Oct  4 03:46:13 2026 GMT
  host: www.rentacenter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:54:48 2026 GMT
  host: www.acima.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: epay.rentacenter.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''epay.rentac'
kind: domain-security
layout: security
method: probed
name: Rent A Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rent-A-Center, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rent-A-Center
provider_slug: rent-a-center
slug: rent-a-center-domain-security
source_filename: rent-a-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentacenter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:46:13 2026 GMT\n  hsts: null\n- host: www.acima.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:54:48 2026 GMT\n  hsts: null\n- host: epay.rentacenter.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''epay.rentac'\n  hsts: null\ndomains:\n- domain: rentacenter.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: acima.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rent-a-center/refs/heads/main/security/rent-a-center-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Lease-To-Own
- Consumer Finance
- Electronics
- Furniture
- Fortune 1000
---
