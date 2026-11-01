---
description: ''
domains:
- caa:
  - 128 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sunsama.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: sunsama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sunsama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunsama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sunsama
provider_slug: sunsama
slug: sunsama-domain-security
source_filename: sunsama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunsama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sunsama.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sunsama/security/sunsama-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Productivity
- Task Management
- Calendar Integration
- Remote Work
---
