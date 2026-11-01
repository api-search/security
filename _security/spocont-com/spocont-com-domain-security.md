---
description: ''
domains:
- caa:
  - ifr.spocont.com.
  - domain.par.clever-cloud.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: spocont.com
  spf: true
hosts:
- cert_expires: Dec  5 02:37:26 2026 GMT
  host: spocont.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spocont Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for spocont-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: spocont-com
provider_slug: spocont-com
slug: spocont-com-domain-security
source_filename: spocont-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spocont.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 02:37:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spocont.com\n  dnssec: true\n  caa:\n  - ifr.spocont.com.\n  - domain.par.clever-cloud.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/spocont-com/security/spocont-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ContactCenter
- Automation
- CloudPlatform
- API
---
