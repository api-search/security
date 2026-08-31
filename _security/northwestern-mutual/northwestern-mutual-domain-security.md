---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: northwesternmutual.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.northwesternmutual.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Northwestern Mutual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northwestern Mutual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Northwestern Mutual
provider_slug: northwestern-mutual
slug: northwestern-mutual-domain-security
source_filename: northwestern-mutual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.northwesternmutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: northwesternmutual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northwestern-mutual/refs/heads/main/security/northwestern-mutual-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Life-Insurance
- Financial-Services
- Wealth-Management
- Annuities
- Investment-Management
- Fortune 500
---
