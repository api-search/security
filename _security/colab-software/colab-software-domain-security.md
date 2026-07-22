---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@colabsoftware.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: colabsoftware.com
  spf: true
hosts:
- cert_expires: Oct  3 05:17:44 2026 GMT
  host: www.colabsoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colab Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoLab Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CoLab Software
provider_slug: colab-software
slug: colab-software-domain-security
source_filename: colab-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colabsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:17:44 2026 GMT\n  hsts: false\ndomains:\n- domain: colabsoftware.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@colabsoftware.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colab-software/refs/heads/main/security/colab-software-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Design Review
- Engineering Collaboration
- CAD
- Product Development
- AI
- PLM
- Manufacturing
---
