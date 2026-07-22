---
description: ''
domains:
- caa:
  - 0 iodef "mailto:infosecalerts@circana.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: false
  domain: retailsolutions.com
  spf: true
hosts:
- host: www.retailsolutions.com
  https: false
kind: domain-security
layout: security
method: probed
name: Retail Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retail Solutions, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Retail Solutions
provider_slug: retail-solutions
slug: retail-solutions-domain-security
source_filename: retail-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.retailsolutions.com\n  https: false\ndomains:\n- domain: retailsolutions.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:infosecalerts@circana.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retail-solutions/refs/heads/main/security/retail-solutions-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Cloud
- Retail
---
