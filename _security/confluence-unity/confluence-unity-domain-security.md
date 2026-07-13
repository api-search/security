---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "web.com"
  - 0 iodef "mailto:security@confluence.com"
  - 0 issue "confluencetrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: confluence.com
  spf: true
hosts:
- cert_expires: Sep 28 18:14:14 2026 GMT
  host: www.confluence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confluence Unity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confluence Unity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Confluence Unity
provider_slug: confluence-unity
slug: confluence-unity-domain-security
source_filename: confluence-unity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.confluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: confluence.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"web.com\"\n  - 0 iodef \"mailto:security@confluence.com\"\n  - 0 issue \"confluencetrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluence-unity/refs/heads/main/security/confluence-unity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Asset Management
- Asset Servicing
- Financial Reporting
- Fund Administration
- Investment Management
- Performance Analytics
- Regulatory Reporting
- SaaS
---
