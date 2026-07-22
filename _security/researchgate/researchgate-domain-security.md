---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@researchgate.net"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: researchgate.net
  spf: true
hosts:
- cert_expires: Sep 16 13:02:22 2026 GMT
  host: www.researchgate.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Researchgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ResearchGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ResearchGate
provider_slug: researchgate
slug: researchgate-domain-security
source_filename: researchgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.researchgate.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:02:22 2026 GMT\n  hsts: null\ndomains:\n- domain: researchgate.net\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@researchgate.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/researchgate/refs/heads/main/security/researchgate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer Internet
- Research
- Academic
- Social Network
- Publishing
- Science
---
