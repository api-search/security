---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: distributionos.dev
  spf: true
hosts:
- cert_expires: Jan 20 12:52:02 2027 GMT
  host: distributionos.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DistributionOS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DistributionOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DistributionOS
provider_slug: distributionos-dev
slug: distributionos-dev-domain-security
source_filename: distributionos-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distributionos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 12:52:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: distributionos.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/distributionos-dev/security/distributionos-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Analytics
- MCP
---
