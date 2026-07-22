---
description: ''
domains:
- caa:
  - pki.goog
  - sectigo.com
  - amazon.com
  - certainly.com
  - digicert.com
  - letsencrypt.org
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: optro.ai
  spf: true
- caa:
  - letsencrypt.org
  - pki.goog
  - sectigo.com
  - amazon.com
  - certainly.com
  - digicert.com
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auditboard.com
  spf: true
hosts:
- cert_not_after: '2026-09-18'
  host: optro.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 300
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_not_after: '2026-10-02'
  host: developer.auditboard.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auditboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AuditBoard, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AuditBoard
provider_slug: auditboard
slug: auditboard-domain-security
source_filename: auditboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: dig + openssl/curl HEAD against live hosts\nnote: AuditBoard rebranded to Optro; primary web host is now optro.ai. developer.auditboard.com serves the (login-gated) developer portal.\nhosts:\n  - host: optro.ai\n    https: true\n    tls_version: TLSv1.3\n    cert_not_after: '2026-09-18'\n    hsts: true\n    hsts_max_age: 300\n    hsts_include_subdomains: true\n    hsts_preload: true\n  - host: developer.auditboard.com\n    https: true\n    tls_version: TLSv1.3\n    cert_not_after: '2026-10-02'\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: false\n    hsts_preload: false\ndomains:\n  - domain: optro.ai\n    dnssec: false\n    caa: ['pki.goog', 'sectigo.com', 'amazon.com', 'certainly.com', 'digicert.com', 'letsencrypt.org']\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n  - domain: auditboard.com\n    dnssec: false\n    caa: ['letsencrypt.org', 'pki.goog', 'sectigo.com', 'amazon.com', 'certainly.com',\
  \ 'digicert.com']\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auditboard/refs/heads/main/security/auditboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GRC
- Governance Risk Compliance
- Audit Management
- Risk Management
- Compliance
- Internal Audit
- SOX
- Cybersecurity Compliance
- ESG
- AI Governance
- SaaS
---
