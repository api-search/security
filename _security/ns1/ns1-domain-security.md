---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ns1.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nsone.net
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: ns1.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 03:39:01 2027 GMT
  host: api.nsone.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ns1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NS1, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NS1
provider_slug: ns1
slug: ns1-domain-security
source_filename: ns1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ns1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nsone.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  5 03:39:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ns1.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nsone.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ns1/refs/heads/main/security/ns1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Networking
- DNS
- Managed DNS
- Traffic Management
- DDI
- API
- Infrastructure
---
