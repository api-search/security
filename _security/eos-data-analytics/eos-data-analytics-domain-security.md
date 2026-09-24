---
description: ''
domains:
- caa:
  - 0 iodef "mailto:admins@eosda.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eos.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: eos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eos Data Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EOS Data Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EOS Data Analytics
provider_slug: eos-data-analytics
slug: eos-data-analytics-domain-security
source_filename: eos-data-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eos.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admins@eosda.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eos-data-analytics/refs/heads/main/security/eos-data-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Satellite
- Analytics
- Agriculture
- Environmental
---
