---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: launchmetrics.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: launchmetrics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: nap.launchmetrics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Launchmetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launchmetrics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Launchmetrics
provider_slug: launchmetrics
slug: launchmetrics-domain-security
source_filename: launchmetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launchmetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n- host: nap.launchmetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: launchmetrics.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchmetrics/refs/heads/main/security/launchmetrics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- Marketing
- Public Relations
- Media Monitoring
- Social Media
- Analytics
- Fashion
- Luxury
- Beauty
- Brand Performance
- Event Management
- Search
---
