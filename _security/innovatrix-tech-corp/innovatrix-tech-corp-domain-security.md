---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getsahl.io
  spf: true
hosts:
- cert_expires: Oct 17 11:01:34 2026 GMT
  host: getsahl.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Innovatrix Tech Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innovatrix Tech, Corp., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Innovatrix Tech, Corp.
provider_slug: innovatrix-tech-corp
slug: innovatrix-tech-corp-domain-security
source_filename: innovatrix-tech-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsahl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: getsahl.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovatrix-tech-corp/refs/heads/main/security/innovatrix-tech-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GRC
- Compliance
- Governance
- Risk
- Security
- Regulatory
- Audit
- MENA
- Artificial Intelligence
---
