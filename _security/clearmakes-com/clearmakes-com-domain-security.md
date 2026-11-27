---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clearmakes.com
  spf: true
hosts:
- cert_expires: Dec 17 18:39:42 2026 GMT
  host: clearmakes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: clearmakes-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for clearmakes-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: clearmakes-com
provider_slug: clearmakes-com
slug: clearmakes-com-domain-security
source_filename: clearmakes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearmakes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 18:39:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clearmakes.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clearmakes-com/security/clearmakes-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Service
- Remote Teams
---
