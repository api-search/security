---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: berkley.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: berkleysig.com
  spf: true
hosts:
- cert_expires: Jul 14 14:00:45 2026 GMT
  host: www.berkley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:56:07 2026 GMT
  host: myberkley.berkleysig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 14 14:00:46 2026 GMT
  host: berkleynet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wr Berkley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for W. R. Berkley, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: W. R. Berkley
provider_slug: wr-berkley
slug: wr-berkley-domain-security
source_filename: wr-berkley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berkley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 14 14:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myberkley.berkleysig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:56:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: berkleynet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 14 14:00:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: berkley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: berkleysig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wr-berkley/refs/heads/main/security/wr-berkley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Property And Casualty
- Commercial Lines
- Reinsurance
- Workers Compensation
- Fortune 500
---
