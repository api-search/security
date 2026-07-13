---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2209672455"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dana.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: danaaftermarket.com
  spf: true
hosts:
- cert_expires: Aug 29 14:17:14 2026 GMT
  host: www.dana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.danaaftermarket.com
  https: false
- host: api.danaaftermarket.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dana Incorporated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dana Incorporated, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dana Incorporated
provider_slug: dana-incorporated
slug: dana-incorporated-domain-security
source_filename: dana-incorporated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.danaaftermarket.com\n  https: false\n- host: api.danaaftermarket.com\n  https: false\ndomains:\n- domain: dana.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2209672455\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: danaaftermarket.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dana-incorporated/refs/heads/main/security/dana-incorporated-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aftermarket
- Auto Parts
- Automotive
- Drivetrain
- Electrified Propulsion
- Fortune 500
---
