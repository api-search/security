---
description: ''
domains:
- caa:
  - 0 iodef "mailto:cody@software.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: software.com
  spf: true
hosts:
- host: software.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Software Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software
provider_slug: software-com
slug: software-com-domain-security
source_filename: software-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: software.com\n  https: false\ndomains:\n- domain: software.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:cody@software.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/software-com/security/software-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- Software
- API
- Integration
- Enterprise
---
