---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:netops@actifio.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actifio.com
  spf: true
hosts:
- cert_expires: Sep 21 08:42:03 2026 GMT
  host: www.actifio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Actifio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actifio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Actifio
provider_slug: actifio
slug: actifio-domain-security
source_filename: actifio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actifio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:42:03 2026 GMT\n  hsts: false\ndomains:\n- domain: actifio.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:netops@actifio.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actifio/refs/heads/main/security/actifio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Management
- Backup
- Disaster Recovery
- Copy Data Management
- Business Continuity
- Cloud
- Enterprise Storage
---
