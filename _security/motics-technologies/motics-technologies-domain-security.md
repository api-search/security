---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@motics.ai"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: motics.ai
  spf: true
hosts:
- cert_expires: Oct  7 17:00:31 2026 GMT
  host: www.motics.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motics Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motics Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Motics Technologies
provider_slug: motics-technologies
slug: motics-technologies-domain-security
source_filename: motics-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.motics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:00:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: motics.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@motics.ai\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motics-technologies/refs/heads/main/security/motics-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- AI Agents
- Clinical Documentation
- Health Technology
- Medical
- Automation
- United Kingdom
---
