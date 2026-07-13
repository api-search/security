---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hippo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firstconnectinsurance.com
  spf: true
hosts:
- cert_expires: Aug 10 15:17:31 2026 GMT
  host: www.hippo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:01:26 2026 GMT
  host: www.firstconnectinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 15:24:38 2026 GMT
  host: portal.firstconnectinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hippo Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hippo Insurance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hippo Insurance
provider_slug: hippo-insurance
slug: hippo-insurance-domain-security
source_filename: hippo-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 15:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.firstconnectinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:01:26 2026 GMT\n  hsts: false\n- host: portal.firstconnectinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:24:38 2026 GMT\n  hsts: false\ndomains:\n- domain: hippo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: firstconnectinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hippo-insurance/refs/heads/main/security/hippo-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Homeowners
- Insurtech
- Smart Home
- Agents
- MGA
- Embedded Insurance
- Carrier
---
