---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:yuval@ilumex.ai"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: illumex.ai
  spf: true
hosts:
- host: illumex.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Illumex Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for illumex, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: illumex
provider_slug: illumex-ai
slug: illumex-ai-domain-security
source_filename: illumex-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: illumex.ai\n  https: false\ndomains:\n- domain: illumex.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:yuval@ilumex.ai\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/illumex-ai/security/illumex-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- AI
- Data Management
- Enterprise
- Analytics
---
