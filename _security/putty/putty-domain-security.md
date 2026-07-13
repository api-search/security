---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: putty.org
  spf: true
hosts:
- cert_expires: Sep 26 22:33:48 2026 GMT
  host: www.putty.org
  hsts: true
  hsts_max_age: 99979997
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Putty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PuTTY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PuTTY
provider_slug: putty
slug: putty-domain-security
source_filename: putty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.putty.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 22:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 99979997\ndomains:\n- domain: putty.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/putty/refs/heads/main/security/putty-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Network Tools
- Open Source
- Remote Access
- SSH
- Terminal
---
