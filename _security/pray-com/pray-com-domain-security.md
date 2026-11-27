---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pray.com
  spf: true
hosts:
- cert_expires: May 25 11:31:09 2027 GMT
  host: pray.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PRAY.COM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PRAY.COM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PRAY.COM
provider_slug: pray-com
slug: pray-com-domain-security
source_filename: pray-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 25 11:31:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pray.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pray-com/security/pray-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Faith
- Prayer
- Bible
- Podcasts
---
