---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@revealdata.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nexlp.com
  spf: true
hosts:
- host: nexlp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nexlp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NexLP, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NexLP
provider_slug: nexlp
slug: nexlp-domain-security
source_filename: nexlp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexlp.com\n  https: false\ndomains:\n- domain: nexlp.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@revealdata.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexlp/refs/heads/main/security/nexlp-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Legal
- LegalTech
- Artificial Intelligence
- eDiscovery
- Compliance
- Investigations
- Acquired
---
