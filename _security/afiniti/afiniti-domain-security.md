---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:domains@afiniti.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: afiniti.com
  spf: true
hosts:
- cert_expires: Sep 16 04:42:39 2026 GMT
  host: www.afiniti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Afiniti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afiniti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Afiniti
provider_slug: afiniti
slug: afiniti-domain-security
source_filename: afiniti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afiniti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:42:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: afiniti.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:domains@afiniti.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afiniti/refs/heads/main/security/afiniti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Contact Center
- Customer Experience
- Machine Learning
- Enterprise AI
- Call Routing
- CCaaS
---
