---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:tls@libravatar.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: libravatar.org
  spf: true
hosts:
- cert_expires: Jan 19 05:07:33 2027 GMT
  host: libravatar.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Libravatar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Libravatar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Libravatar
provider_slug: libravatar
slug: libravatar-domain-security
source_filename: libravatar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: libravatar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 05:07:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: libravatar.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:tls@libravatar.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/libravatar/security/libravatar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Avatar
- OpenSource
- Federated
- API
---
