---
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 iodef "mailto:infosecnotice@smud.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smud.org
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.smud.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smud Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sacramento Municipal Utility District (SMUD), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sacramento Municipal Utility District (SMUD)
provider_slug: smud-org
slug: smud-org-domain-security
source_filename: smud-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smud.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: smud.org\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:infosecnotice@smud.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smud-org/refs/heads/main/security/smud-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Utilities
- Electricity
---
