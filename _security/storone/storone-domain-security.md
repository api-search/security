---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storone.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: onestor.com
  spf: true
hosts:
- cert_expires: Oct  2 20:04:17 2026 GMT
  host: www.storone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 09:02:42 2026 GMT
  host: docs.onestor.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StorONE, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StorONE
provider_slug: storone
slug: storone-domain-security
source_filename: storone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:04:17 2026 GMT\n  hsts: false\n- host: docs.onestor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 09:02:42 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: storone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: onestor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storone/refs/heads/main/security/storone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Storage
- Enterprise Storage
- Software Defined Storage
- Data Management
- Infrastructure
- Block Storage
- File Storage
- Object Storage
- Backup
- Replication
- Snapshots
- Company
---
