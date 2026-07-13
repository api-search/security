---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acl.gov
  spf: true
hosts:
- cert_expires: Nov 26 21:01:36 2026 GMT
  host: acl.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 27 23:59:59 2026 GMT
  host: agid.acl.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Administration For Community Living Acl  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Administration for Community Living (ACL), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Administration for Community Living (ACL)
provider_slug: administration-for-community-living-acl-
slug: administration-for-community-living-acl--domain-security
source_filename: administration-for-community-living-acl--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acl.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 21:01:36 2026 GMT\n  hsts: false\n- host: agid.acl.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acl.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administration-for-community-living-acl-/refs/heads/main/security/administration-for-community-living-acl--domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Aging
- Federal Government
- Healthcare
- Disability
- Independent Living
- Open Data
- Social Services
---
