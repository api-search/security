---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spacerickshaw.com
  spf: false
hosts:
- cert_expires: Dec 12 18:03:01 2026 GMT
  host: spacerickshaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spacerickshaw Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalyx Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Catalyx Space
provider_slug: spacerickshaw-com
slug: spacerickshaw-com-domain-security
source_filename: spacerickshaw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacerickshaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:03:01 2026 GMT\n  hsts: false\ndomains:\n- domain: spacerickshaw.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/spacerickshaw-com/security/spacerickshaw-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
