---
description: ''
domains:
- caa:
  - 0 contactemail "pkiadmin@dell.com"
  - 0 issue "digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9"
  - 0 iodef "mailto:pkiadmin@dell.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dell.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.dell.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EMC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EMC
provider_slug: emc
slug: emc-domain-security
source_filename: emc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: dell.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"pkiadmin@dell.com\"\n  - 0 issue \"digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9\"\n  - 0 iodef \"mailto:pkiadmin@dell.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emc/refs/heads/main/security/emc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Infrastructure
- Data Management
- Data Protection
- Enterprise Storage
- Storage
- Fortune 500
---
