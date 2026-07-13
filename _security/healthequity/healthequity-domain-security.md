---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: healthequity.com
  spf: true
hosts:
- cert_expires: Aug 26 02:30:53 2026 GMT
  host: www.healthequity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 18 01:58:55 2026 GMT
  host: developer.healthequity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.healthequity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthequity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthEquity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HealthEquity
provider_slug: healthequity
slug: healthequity-domain-security
source_filename: healthequity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:30:53 2026 GMT\n  hsts: null\n- host: developer.healthequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 18 01:58:55 2026 GMT\n  hsts: null\n- host: api.healthequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: healthequity.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthequity/refs/heads/main/security/healthequity-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- HSA
- Benefits
---
