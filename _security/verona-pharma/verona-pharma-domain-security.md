---
description: ''
domains:
- caa:
  - 0 iodef "mailto:soc@veronapharma.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veronapharma.com
  spf: true
hosts:
- host: www.veronapharma.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verona Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verona Pharma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verona Pharma
provider_slug: verona-pharma
slug: verona-pharma-domain-security
source_filename: verona-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veronapharma.com\n  https: false\ndomains:\n- domain: veronapharma.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:soc@veronapharma.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/verona-pharma/security/verona-pharma-domain-security.yml
summary_line: DMARC
tags:
- Company
---
