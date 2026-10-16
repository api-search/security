---
description: ''
domains:
- caa:
  - 0 iodef "mailto:core@6estates.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 6estates.com
  spf: true
hosts:
- cert_expires: Jan  8 09:39:07 2027 GMT
  host: 6estates.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 6Estates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6Estates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 6Estates
provider_slug: 6estates
slug: 6estates-domain-security
source_filename: 6estates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6estates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 09:39:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 6estates.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:core@6estates.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6estates/refs/heads/main/security/6estates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Enterprise
- Automation
- Finance
---
