---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: orsted.com
  spf: true
hosts:
- cert_expires: Dec 20 10:52:39 2026 GMT
  host: orsted.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orsted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orsted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Orsted
provider_slug: orsted
slug: orsted-domain-security
source_filename: orsted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orsted.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 10:52:39 2026 GMT\n  hsts: null\ndomains:\n- domain: orsted.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orsted/refs/heads/main/security/orsted-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Energy
- Renewable
- OffshoreWind
- Sustainability
- Denmark
- Company
---
