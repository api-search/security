---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@craigslist.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: craigslist.org
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.craigslist.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Craigslist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craigslist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Craigslist
provider_slug: craigslist
slug: craigslist-domain-security
source_filename: craigslist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.craigslist.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: craigslist.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@craigslist.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craigslist/refs/heads/main/security/craigslist-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Classifieds
- Marketplace
- Jobs
- Housing
- Community
---
