---
description: ''
domains:
- caa:
  - 128 iodef "mailto:input@desec.io"
  - 128 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/1909605"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: desec.io
  spf: true
hosts:
- cert_expires: Jan 10 14:35:35 2027 GMT
  host: desec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Desec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for deSEC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: deSEC
provider_slug: desec
slug: desec-domain-security
source_filename: desec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:35:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: desec.io\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:input@desec.io\"\n  - 128 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/1909605\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/desec/security/desec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DNS
- Security
- OpenSource
- FreeService
- Company
---
