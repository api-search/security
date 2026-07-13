---
description: ''
domains:
- caa:
  - 128 issue "globalsign.com"
  - 128 issuewild "globalsign.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xkcd.com
  spf: true
hosts:
- cert_expires: Jan  9 22:00:18 2027 GMT
  host: xkcd.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xkcd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xkcd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: xkcd
provider_slug: xkcd
slug: xkcd-domain-security
source_filename: xkcd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xkcd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 22:00:18 2027 GMT\n  hsts: false\ndomains:\n- domain: xkcd.com\n  dnssec: false\n  caa:\n  - 128 issue \"globalsign.com\"\n  - 128 issuewild \"globalsign.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xkcd/refs/heads/main/security/xkcd-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Games And Comics
- Public APIs
---
