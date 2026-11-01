---
description: ''
domains:
- caa:
  - 128 issue "amazonaws.com"
  - 128 issue "amazontrust.com"
  - 128 issue "digicert.com"
  - 128 issue "amazon.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firefox.com
  spf: true
hosts:
- cert_expires: Jan  9 17:18:19 2027 GMT
  host: accounts.firefox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mozilla Accounts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mozilla accounts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mozilla accounts
provider_slug: mozilla-accounts
slug: mozilla-accounts-domain-security
source_filename: mozilla-accounts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accounts.firefox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 17:18:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firefox.com\n  dnssec: false\n  caa:\n  - 128 issue \"amazonaws.com\"\n  - 128 issue \"amazontrust.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mozilla-accounts/security/mozilla-accounts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authentication
- Identity
- Mozilla
- OpenSource
---
