---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:admins@koongo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: koongo.com
  spf: true
hosts:
- cert_expires: Jan  5 01:53:27 2027 GMT
  host: koongo.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Koongo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koongo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Koongo
provider_slug: koongo-com
slug: koongo-com-domain-security
source_filename: koongo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koongo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 01:53:27 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: koongo.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:admins@koongo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/koongo-com/security/koongo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Marketplace
- Automation
- Integration
- Multi-Channel
---
