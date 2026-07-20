---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "gandi.net"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: causaly.com
  spf: true
hosts:
- cert_expires: Sep 22 21:11:00 2026 GMT
  host: www.causaly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Causaly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Causaly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Causaly
provider_slug: causaly
slug: causaly-domain-security
source_filename: causaly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.causaly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:11:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: causaly.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"gandi.net\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causaly/refs/heads/main/security/causaly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Life Sciences
- Biomedical
- Drug Discovery
- Knowledge Graph
- Pharmaceutical
- Research
- Agentic AI
---
